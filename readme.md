# Passportjs

* Authentication
* Federation Authentication : 많은 사람들이 이미 회원가입된 정보를 이용해서 지금 로그인한 사람이 직접 회원가입해서 정보를 확인하는 것이아니라 네이버나 카카오를 통해 정보를 얻어오는 방식.

### 설치

```
npm install --save passport passport-local
```

`app_passport_file.js`

```javascript
var passport = require('passport')
  , LocalStrategy = require('passport-local').Strategy;
```

### Middleware

`app_passport_file.js`

```javascript
app.use(passport.initialize());
app.use(passport.session()); //passport를 사용할 때 인증으로 session을 이용함. session 세팅 뒤에 꼭 써야함.
```



