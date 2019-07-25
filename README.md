# 시작
## 개요
    - nodejs + express 를 이용 single page app
    - 간단한 회원가입 기능 구현
    - 간단한 로그인/로그아웃 구현
    - 간단한 게시판 구현

## 개발환경 구성
    >> express --view=ejs project001
    >> npm i
    >> npm i --save-dev nodemon

## index.ejs
    w3shools.com 의 Bootstrap Themes중 Company 코드 적용
    링크 : https://www.w3schools.com/bootstrap/tryit.asp?filename=trybs_theme_company_complete_animation

## 하단의 contact section 복사하여 가입 폼 및 로그인 폼 작성
    - style유지를 위해 class는 그대로 둔다
    - style유지를 위해 tag-tree구조를 바꾸지 않는다
    - tag들의 id 중복을 피하기 위해 id를 목적에 맞게 변경

## jquery를 이용한 sign up 버튼 이벤트 구현
    1) index.ejs의 <head>내부에 jquery cdn 등록 확인

```html
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.4.1/jquery.min.js"></script>
```
    
    2) index.ejsdml <head>내부에 사용 할 스크립트 등록 후
        - 본 프로젝트 폴더 구조의 public/javascripts/ 에 signup.js 생성
```html
<script src="javascripts/signup.js"></script>
```

    3) signup.js 작성 (작동테스트)
```javascript
$(document).ready(() => {
    $('#ID_btn_signup').click(() => {
        alert();
    });
});
```
