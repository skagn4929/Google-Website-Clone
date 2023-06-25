# Google-Website-Clone
**HTML과 CSS를 사용하여 넷플릭스 웹사이트 클론을 만들었습니다.**
- https://skagn4929.github.io/Google-Website-Clone/

![구글](https://github.com/skagn4929/Google-Website-Clone/assets/134206709/45a71a41-041a-4216-a970-b61a9b010bcb)

---

## 1. 프로젝트의 동기   
**클론 코딩을 통한 HTML 과 CSS 언어의 학습**

## 2. 프로젝트 주요 내용   
**1. 헤더섹션에 여러 메뉴 버튼과 프로필 아이콘을 만들었습니다.**

![구글1](https://github.com/skagn4929/Google-Website-Clone/assets/134206709/d1062e86-b238-40c2-b96d-0f9071393a4e)

- HTML
```html
    <header>
      <nav class="navbar">
        <ul class="left-items">
          <li>
            <a class="link" href="">Google 정보</a>
          </li>
          <li>
            <a class="link" href="">스토어</a>
          </li>
        </ul>
        <ul class="right-items">
          <li>
            <a class="link" href="">Gmail</a>
          </li>
          <li>
            <a class="link" href="">이미지</a>
          </li>
          <li>
            <div class="circle-shadow">
              <a class="menu-icon" href=""><i class="fa-solid fa-bars"></i></a>
            </div>
          </li>
          <li>
            <div class="circle-shadow">
              <a class="user-icon" href=""><span>K</span></a>
            </div>
          </li>
        </ul>
      </nav>
    </header>
```
- CSS
```css
header {
  height: 60px;
}

.navbar {
  height: 100%;
  width: 100%;
  padding: 10px 20px;
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.navbar ul {
  display: flex;
  align-items: center;
  font-size: 14px;
}

.navbar ul.left-items li {
  margin-right: 15px;
}

.navbar ul.right-items li {
  margin-left: 15px;
}

.navbar ul li a {
  color: black;
}

.link:hover {
  text-decoration: underline;
}

.circle-shadow {
  height: 40px;
  width: 40px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
}

.circle-shadow:hover {
  background-color: rgba(0, 0, 0, 0.1);
}

.menu-icon,
.user-icon span {
  font-size: 18px;
}

.user-icon span {
  color: white;
}

.user-icon {
  background-color: green;
  height: 30px;
  width: 30px;
  border-radius: 50%;
  text-align: center;
  line-height: 30px;
}
```

---

**2. 본문 중앙에 구글 로고와 검색창 그에 맞는 아이콘을 넣어 만들었습니다.**

![구글2](https://github.com/skagn4929/Google-Website-Clone/assets/134206709/91743d09-b445-453a-ac94-e2cfeebf7672)

- HTML
```html
    <section class="content-section">
      <div class="content-wrapper">
        <img class="logo-img" src="./images/logo.jpg" alt="Google logo Image" />
        <div class="search-bar">
          <i class="fa-solid fa-magnifying-glass"></i>
          <input class="search-input" type="text" />
          <i class="fa-solid fa-keyboard"></i>
          <i class="fa-solid fa-microphone"></i>
        </div>
        <div class="search-btns">
          <button class="google-search-btn">Google 검색</button>
          <button class="lucky-search-btn">I'm Feeling Lucky</button>
        </div>
      </div>
    </section>
```
- CSS
```css
.content-section {
  flex-grow: 1;
  display: flex;
  justify-content: center;
  align-items: center;
}

.content-wrapper {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding-bottom: 100px;
}

.logo-img {
  width: 300px;
  margin-bottom: 20px;
}

.search-bar {
  border: 1px solid lightgray;
  width: 600px;
  height: 45px;
  border-radius: 30px;
  display: flex;
  align-items: center;
  padding-left: 15px;
}

.search-bar:hover {
  box-shadow: 0px 0px 4px 0px #b5b5b5;
}

.search-bar i {
  font-size: 18px;
  color: gray;
  margin-right: 15px;
  cursor: pointer;
}

.search-bar input {
  flex-grow: 1;
  height: 30px;
  margin-right: 15px;
  font-size: 16px;
  border: none;
}

.search-bar input:focus {
  outline: none;
}

.search-btns {
  margin-top: 20px;
}

.search-btns button {
  height: 40px;
  font-size: 14px;
  border: none;
  border-radius: 5px;
  margin-left: 10px;
  color: black;
  background-color: #f2f3f4;
}

.search-btns button:hover {
  border: 1px solid lightgray;
}

.google-search-btn {
  width: 105px;
}

.lucky-search-btn {
  width: 140px;
}
```

---

**3. 바닥글에 해당 국가와 기타 링크 버튼을 만들었습니다.**

![구글3](https://github.com/skagn4929/Google-Website-Clone/assets/134206709/d118a867-2eac-403b-9a59-6b6315b68dcc)

- HTML
```html
    <footer>
      <div class="footer-content upper-footer">
        <p>대한민국</p>
      </div>
      <div class="footer-content lower-footer">
        <ul class="lower-left-footer">
          <li>
            <a href="">광고</a>
          </li>
          <li>
            <a href="">비즈니스</a>
          </li>
          <li>
            <a href="">검색의 원리</a>
          </li>
        </ul>
        <ul class="lower-right-footer">
          <li>
            <a href="">개인정보처리방침</a>
          </li>
          <li>
            <a href="">약관</a>
          </li>
          <li>
            <a href="">설정</a>
          </li>
        </ul>
      </div>
    </footer>
```
- CSS
```css
footer {
  background-color: #f2f2f2;
  height: 100px;
}

.footer-content {
  display: flex;
  align-items: center;
  padding: 20px;
}

.upper-footer {
  height: 50%;
  border-bottom: 1px solid lightgray;
}

.upper-footer p {
  color: gray;
  font-size: 14px;
}

.lower-footer {
  height: 50%;
  display: flex;
  justify-content: space-between;
}

.lower-footer ul li a {
  font-size: 14px;
  color: grey;
}

.lower-footer ul li a:hover {
  text-decoration: underline;
}

.lower-left-footer {
  display: flex;
}

.lower-left-footer li {
  margin-right: 15px;
}

.lower-right-footer {
  display: flex;
}

.lower-right-footer li {
  margin-left: 15px;
}
```

---
### 참고
- https://www.google.co.kr/ - 이미지 참고

- https://fontawesome.com/ - 아이콘 참고








