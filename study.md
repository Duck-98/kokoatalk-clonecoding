# 학습 내용정리

## css
position: absolute는 가장 가까운 relative를 가진 부모 기준으로 움직인다.
```css
.nav__link{
    position: relative;
    color: #2E363E;
}
.nav__notification{
    background-color: tomato;
    width: 30px;
    height: 30px;
    border-radius: 15px;
    display: flex;
    justify-content: center;
    align-items: center;
    color: white;
    font-weight: 600;
    position: absolute;
    left : 15px;
    bottom: 15px;
}
```
```html
<a class="nav__link" href="#">
    <span class="nav__notification">1</span>
</a>
```
위와 같은 상황에서 *nav__ontification*의 위치를 바꾸고 싶다면, 부모 클래스인 *nav__link*의  position을 relative로 기준을 잡아 위치를 바꿔줘야한다.