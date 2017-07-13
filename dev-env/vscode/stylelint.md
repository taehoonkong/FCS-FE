# 1. install stylelint & stylelint-config-standard

```bash
$ npm install -g stylelint
$ npm install stylelint-config-standard --save-dev
```

# 2. install Stylelint VSCode extention

# 3. VSCode settings

Windows: File > Preferences > Settings 
Mac: Code > Preferences > Settings on Mac

아래의 설정을 추가한다.

```json
{
  "css.validate": false,
  "scss.validate": false
}
```

# 4. .stylelintrc

기본 룰셋을 사용하고 필요에 따라 변경한다.

```json
{
  "extends": "stylelint-config-standard",
   "rules": {
     // Add your rules 
     // Rules: https://stylelint.io/user-guide/rules/
   }
}
```

# 5. Reference

- [stylelint](https://github.com/stylelint/stylelint)
