# SASS VSCode 사용법

#### 설치

- 필수 확장프로그램 설치

  - live sass compiler
  - live server
  - sass

- VSCode 기본 설정

  - 단축키

    - mac => command + shift + p 입력 후 settings.json 입력
    - window => Ctrl + p 입력 후 settings.json 입력

  - settings.json 파일에 붙여 넣기
    ````
    // 컴파일 포맷 방식 작성.
    "liveSassCompile.settings.formats": [
    {
    "format": "expanded",
    "extensionName": ".css",
    "savePath": "~/../css"
    },
    // min 파일 공백이 없는 css 파일
    { "format": "compressed", "extensionName": ".min.css", "savePath": "~/../css" }
    ],
    // map 파일 사용 유무(Default : true) - 소스맵 사용안할 경우 false로 설정
    "liveSassCompile.settings.generateMap": false,
    // 자동 밴더 프리픽스 사용하게 해줌.
    "liveSassCompile.settings.autoprefix": ["> 1%", "last 2 versions"],
    // 특정 파일만 컴파일 할 때 [파일 경로와 파일 명]
    "liveSassCompile.settings.includeItems": ["scss/*.scss"],
       ```
    ````
