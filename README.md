# Лабораторная работа XII

## Task
- [X] Написать программу на *C++* обеспечивающую асинхронный запрос по заданному *URL* к *HTTPS* серверу на получение кода доступа.

Сборка проекта:
```ShellSession
$ cmake -H. -B_build -DCMAKE_INSTALL_PREFIX=_install
$ cmake --build _build --target install
```

Пример работы программы:
```ShellSession
$ ./cget https://yandex.ru
Response answer == 200
```

## Links
protocols:
- [HTTP](https://ru.wikipedia.org/wiki/HTTP)

documentaion:
- [CURL library](https://curl.haxx.se/libcurl/c/)
- [Boost.Asio](http://www.boost.org/doc/libs/1_65_1/doc/html/boost_asio.html)

hunter:
- [CURL](https://docs.hunter.sh/en/latest/packages/pkg/CURL.html)
- [OpenSSL](https://docs.hunter.sh/en/latest/packages/pkg/OpenSSL.html)
- [Boost](https://docs.hunter.sh/en/latest/packages/pkg/Boost.html)

examples:
- [request](https://curl.haxx.se/libcurl/c/https.html)
- [response](https://curl.haxx.se/libcurl/c/CURLINFO_RESPONSE_CODE.html)
- [client](https://github.com/CloudPolis/webdav-client-cpp)
