# 1. Intro

Browsersync는 다양한 브라우저에서 웹페이지를 테스트할 수 있는 도구이다. 이름에서 알 수 있듯이 파일이 변경되면 자동으로 브라우저를 동기화해주는 프로그램이다.

# 2. install Browsersync

```bash
$ npm install -g browser-sync
$ browser-sync --version
2.18.12
```

# 3. Start Browsersync

```bash
$ cd <project-folder>
## Browsersync Command Line Usage
## https://www.browsersync.io/docs/command-line
$ browser-sync start --server --files "*.html, css/*.css, js/*.js"
```

# 3. Reference

- [Browsersync](https://www.browsersync.io/)

- [크로스 브라우저 테스트에 편리한 Browsersync](https://blog.outsider.ne.kr/1216)
