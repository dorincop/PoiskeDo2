더시드 엔진 (구 프론트엔드 기준) 모방 프로젝트.  
< "엔진 내부 UI는 상관없음." ( https://feedback.theseed.io/posts/280 ) >  
테스트 서버 - https://go2021.glitch.me

나무픽스와 거의 호환된다.

## 기초 사용 방법
- skins 디렉토리를 만든다.
  - [buma](https://github.com/LiteHell/theseed-skin-buma/tree/d77eef50a77007da391c5082b4b94818db372417), [liberty](https://github.com/namuwiki/theseed-skin-liberty/tree/153cf78f70206643ec42e856aff8280dc21eb2c0) 등 원하는 스킨을 내려받고 skins 디렉토리에 스킨 이름으로 하위디렉토리를 만들어 복사한다.
- `npm i`를 실행한다.
- `node server`를 실행한다.

## 숨겨진 설정
- config.json 수정으로 숨겨진 설정을 제어할 수 있다.
  - `disable_email`: (기본값 false) 전자우편 인증을 끈다.
  - `disable_login_history`: (기본값 false) 로그인 내역을 기록하지 않게 한다.
  - `use_external_js`: (기본값 false) theseed.js, jQuery 등을 [theseed.io](https://theseed.io)에서 불러온다.
  - `use_external_css`: (기본값 false) wiki.css 등을 [theseed.io](https://theseed.io)에서 불러온다.
  - `allow_account_deletion`: (기본값 false) 계정 탈퇴를 허용한다.
  - `theseed_version`: (기본값 "4.12.0") [the seed 판올림 기록](https://namu.wiki/w/the%20seed/%EC%97%85%EB%8D%B0%EC%9D%B4%ED%8A%B8#toc)을 참고하여, 모방할 the seed 엔진의 버전을 지정한다(형식 주의! 4.4(X), "4.4"(X), 4.4.1(X), "4.4.1"(O) 문자열 x.y.z 형식으로). 예를 들어, "4.4.2"로 할 경우, v4.4.3에 추가된 쓰레드 주제/문서 변경 기능을 사용할 수 없고, "4.18.0"으로 할 경우 IPACL과 사용자 차단 기능이 비활성화되고 ACLGroup가 활성화되며 ACL에서 이름공간ACL 실행 action를 사용할 수 있다.
