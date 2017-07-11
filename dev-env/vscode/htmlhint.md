# 1. install htmlhint

```bash
$ npm install -g htmlhint
```

# 2. install htmlhint VSCode extention

# 3. .htmlhintrc

.htmlhintrc을 작성하지 않으면 아래의 Defaut Ruleset이 적용된다. 필요에 따라 기본 룰셋을 변경한다.

또는 [HTMLHint](http://htmlhint.com/)에서 필요 설정을 생성한다.

```json
{
    "tagname-lowercase": true,
    "attr-lowercase": true,
    "attr-value-double-quotes": true,
    "doctype-first": true,
    "tag-pair": true,
    "spec-char-escape": true,
    "id-unique": true,
    "src-not-empty": true,
    "attr-no-duplication": true,
    "title-require": true
}
```

# 4. Reference

- [htmlhint](http://htmlhint.com/)

- [htmllint Rules](https://github.com/yaniswang/HTMLHint/wiki/Rules)