# [What you’ll build](https://spring.io/guides/gs/serving-web-content/#_what_you_ll_build)

`greeting`というURIでアクセスできるページを作成していきます。

http://localhost:8080/greeting にGETリクエストを行うと、ブラウザには"Hello, World!"と表示されるようなページです。

```
http://localhost:8080/greeting?name=User
```

先ほどのページに対し、このように末尾に`?name=User`をつけると、"Hello, User!"と表示されます。
