# lecture-scss

### Live Sass Compiler / Live Server 설치

### [live sass compiler docs](https://github.com/ritwickdey/vscode-live-sass-compiler/blob/master/docs/settings.md)

- `box-sizing: border-box`: width와 height 값이 padding과 border를 포함해서 계산돼요.

- `em`: 부모 요소의 폰트 크기를 기준으로 계산됨, 부모 폰트가 20px이면 1.5em → 30px

- `rem`: 루트 요소 (html)의 폰트 크기 기준으로 계산됨, html 폰트가 16px이면 2rem → 32px

| Position | 기준점                    | 문서 흐름 | 스크롤 영향 | z-index |
| -------- | ------------------------- | --------- | ----------- | ------- |
| static   | 기본                      | O         | X           | X       |
| relative | 자신의 원래 위치          | O         | X           | X       |
| absolute | 가까운 위치 지정 조상     | X         | X           | O       |
| fixed    | 브라우저 뷰포트           | X         | O           | O       |
| sticky   | 자신의 위치 + 스크롤 위치 | O         | O           | O       |

- `@mixin btnicon($width: 24, $height: 24)` 과 같이 사용 가능하다.

- `@function` 사용법

```
@function px-to-rem($px, $base: 16) {
  @return ($px / $base) * 1rem;
}

h1 {
  font-size: px-to-rem(24);
}
```

- https://flatuicolors.com/
