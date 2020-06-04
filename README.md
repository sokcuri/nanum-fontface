# Nanum fontface

Nanum fontface는 나눔 글꼴을 self-host 방식으로 프로젝트에 삽입하고 싶을 때 사용할 수 있는 간편 패키지입니다.

Google Fonts에서 제공하는 Early Access 스타일 시트와 WOFF 파일을 그대로 사용하였으며,
여러 파일로 웹 폰트 파일이 분산되어 있어 필요한 폰트 파일만 다운받도록 만들어져 있습니다.

현재 Nanum fontface에서는 `나눔 고딕 (nanum-gothic)`, `나눔 명조 (nanum-myeongjo)`, `나눔 고딕 코딩 (nanum-gothic-coding)`,
`나눔 손글씨 펜체 (nanum-pen-script)`, `나눔 손글씨 붓체 (nanum-brush-script)`를 지원합니다

나눔 글꼴은 네이버에서 배포중인 폰트이며, SIL OPEN FONT LICENSE으로 공개되어 있습니다. 자세한 내용은 아래 나눔 글꼴 공식 사이트를 참고해주세요!
- https://hangeul.naver.com/2017/nanum


## 만든이

- 소쿠릿 (sokcuri)
- https://twitter.com/sokcuri
- https://github.com/sokcuri/nanum-gothic-fontface


## 설치

Nanum Gothic fontface는 NPM을 이용해 설치가 가능합니다.
```
$ npm install nanum-fontface --save
```

## 사용 방법

Vue 또는 React 등 `css-loader`를 사용하는 프로젝트 환경에서는 `import` 또는 `require` 구문을 통해 나눔 글꼴을 바로 임베딩해서 사용할 수 있습니다
* `import 'nanum-fontface/css/nanum-gothic.css'` 또는 `require('nanum-fontface/css/nanum-gothic.css')`

### 지원하는 fontface

* `css/nanum-gothic.css`: 나눔 고딕 (nanum-gothic) fontface
* `css/nanum-myeongjo.css`: 나눔 명조 (nanum-myeongjo) fontface
* `css/nanum-gothic-coding.css`: 나눔 고딕 코딩 (nanum-gothic-coding) fontface
* `css/nanum-pen-script.css`: 나눔 손글씨 펜체 (nanum-pen-script) fontface
* `css/nanum-brush-script.css`: 나눔 손글씨 붓체 (nanum-brush-script) fontface

## 라이센스

나눔글꼴 폰트의 SIL OPEN FONT LICENSE 를 그대로 적용합니다.


## 기타

일반 HTML 페이지에서 사용하고 싶은 경우 Github 페이지에서 Clone or download 초록색 버튼 클릭 후 Download ZIP를 눌러 압축파일을 다운로드하고
루트 폴더에 압축을 푸신 후 스타일시트를 링크해 사용하시면 됩니다.

일반 HTML 페이지에서는 css와 fonts 파일을 루트 폴더에 두고 해당되는 스타일시트를 임포트한 뒤 해당되는 font-family를 지정하면 사용이 가능합니다
* 나눔 명조의 경우
  * 스타일시트 : `<link rel="stylesheet" href="css/nanum-myeongjo.css">`
  * CSS : `font-family: 'nanum-myeongjo'` 지정

나눔 글꼴의 프리뷰는 테스트 페이지 (test.html)에서도 확인 가능합니다
