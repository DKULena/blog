# 1. HTML 구조 설계

프론트엔드 개발자를 지망하며 면접을 보러 다니다 보면 기출 면접 문제가 있죠?
> "브라우저 렌더링 과정에 대해서 설명해주세요"

브라우저 렌더링 과정에 대해서는 추후에 포스팅 하겠지만 우선적으로는 html파일을 읽어오게 됩니다.
```css
main section .login {
            background-color: #711BFF;
        }
```
> *로고 식별을 위해 이미지 쪽에만 css 추가
```html
<body>
    <main>
        <section>
            <span class="intro">더 편리해진 위니브에 오신 걸을 환영합니다.</span>
            <br>
            <div class="login">
                <a href="#">
                    <img src="./src/weniv-logo.png" alt="">
                    <span>로그인</span>
                </a>
            </div>
            <div class="login_info">
                <a href="#"><img src="./src/icon-lock.png" alt="">아이디</a>
                <span>|</span>
                <a href="#"><img src="./src/icon-user.png" alt="">비밀번호 찾기</a>
                <a href="#">회원가입
                </a>
            </div>
        </section>
    </main>
  </body>
```


  </body>
</html>
```

### 결과 창
![login_html](login_html.png)
