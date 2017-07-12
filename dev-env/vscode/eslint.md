# 1. install eslint & Airbnb style guide

[ESLint](http://eslint.org/)

```bash
$ npm install -g eslint
$ cd <project-folder>
$ npm init -y
$ eslint --init
? How would you like to configure ESLint? Use a popular style guide
? Which style guide do you want to follow? Airbnb
? Do you use React? No
? What format do you want your config file to be in? JavaScript
Local ESLint installation not found.
Installing eslint, eslint-plugin-import, eslint-config-airbnb-base
npm notice created a lockfile as package-lock.json. You should commit this f
ile.
npm WARN javascript@1.0.0 No description
npm WARN javascript@1.0.0 No repository field.

+ eslint-config-airbnb-base@11.2.0
+ eslint@3.19.0
+ eslint-plugin-import@2.3.0
added 173 packages in 11.759s
Successfully created .eslintrc.js file in /Users/leeungmo/Desktop/javascript
ESLint was installed locally. We recommend using this local copy instead of
your globally-installed copy.
```

# 2. install ESLint VSCode extention

# 3. VSCode settings

Windows: File > Preferences > Settings 
Mac: Code > Preferences > Settings on Mac

아래의 설정을 추가한다.

```json
{
    "javascript.validate.enable": false
}
```

# 4. .eslintrc.js

1번 과정에서 생성된 룰셋을 필요에 따라 아래와 같이 변경한다.

```javascript
module.exports = {
    "env": {
        "browser": true,
        "commonjs": true,
        "es6": true,
        "node": true,
        "jquery": true
    },
    "extends": "airbnb-base",
    "plugins": [ "import" ],
    "rules": {
        // 0 "off", 1 "warn" 2 "error"
        "no-console": 1,
        "quotes": [ 2, "single" ],
        "no-underscore-dangle": 1,
        "no-plusplus": [ 2, { "allowForLoopAfterthoughts": true }],
        "comma-dangle": [ 2, "never"]
    }
};
```

# 5. [option] eslint-plugin-html

html script 태그 내의 자바스크립트에도 eslint를 적용하고 싶은 경우, eslint-plugin-html 플러그인을 설치한다.

```bash
$ npm install --save-dev eslint-plugin-html
```

.eslintrc.js를 아래와 같이 수정한다.

```javascript
module.exports = {
    ...
    "plugins": [ "import", "html"],
    ...
};
```

# 5. Reference

- [Getting Started with ESLint](http://eslint.org/docs/user-guide/getting-started)

- [Rules](http://eslint.org/docs/rules/)
