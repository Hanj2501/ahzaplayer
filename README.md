# Ahza Player 아자 플레이어

Flutter로 개발된 웹 미디어 플레이어입니다. 

## 기본 설정 

프로젝트를 저장 후 HTML파일이 실행되는 서버에 업도르 하면 됩니다. 

웹 경로는 기본 경로로 설정되어 있습니다. 경로 변경시 **index.html** 파일을 수정하세요.

```
# 기본경로 ex) https://example.com/
<base href="/">


# 변경경로 ex) https://example.com/path/to/
<base href="/path/to/">
```

## 주의사항 

- 웹 브라우저 정책에 따라 일부 재생이 되지 않을 수 있으며 브라우저 설정이 필요합니다. 
  - CORS 허용 설정 : 크롬 확장 프로그램 설치. [Allow CORS: Access-Control-Allow-Origin](https://chrome.google.com/webstore/detail/allow-cors-access-control/lhobafahddgcelffkeicbaginigeejlf)
  - MIX CONTENT 허용 설정 : 사이트 설정 - 해당 도메인 - 안전하지 않은 컨텐츠 - 허용 
  - 다이렉트 재생 기능 사용시 자동재생(Autoplay)이 안되는 경우가 있는데 자동 재생 정책(Autoplay Policy) 참고 

## 기능

- Video.js 기반으로 한 비디오/오디오 플레이어
- HLS, DASH 지원 
- 최근 재생목록 저장 기능 (Browser DB에 저장) 
- LIVE / 해상도 등 표시 
- 배속 기능 
- 키보드 조작 가능 (방향키, Enter/Space, ESC)
- 다이렉트 재생 기능 : GET Parameter 값으로 바로 재생
```
https://hanj2501.github.io/ahzaplayer/#/direct?url=https%3A%2F%2Ftest-streams.mux.dev%2Fx36xhzz%2Fx36xhzz.m3u8
```

