# Bot Challenge Anti Spam Addon V1.0.5
CAPTCHA 없는 스팸 방지 애드온

- 캡차를 사용 하지 않는 스팸 방지 애드온 입니다.
- 회원가입, 글쓰기, 코멘트작성, 쪽지발송 스팸을 전부 차단합니다.
- 사용자를 귀찮게 하지 않습니다. 모든 스팸방지 작업은 백그라운드로 조용히 자동으로 처리됩니다.
- Captcha등 의 다른 스팸방지 애드온과 같이 사용이 가능합니다, 충돌이 일어나지 않습니다.
- JS를 해석 할 줄 모르는 대부분의 악성 스팸 로봇을 전부 차단합니다.
  - 원리 : 클라이언트에 JS HMAC 을 계산하라는 요구를 합니다.
  - 응답 값을 검증하기(안티 스팸봇 테스트)전까지는 회원가입/글쓰기/코멘트작성/쪽지발송 을 차단합니다.
- PHP 5.3 이상에서 정상 작동합니다.
- PHP OpenSSL 관련 기능이 설치되어 있어야 합니다.(대부분(99.9%)의 웹 호스팅 및 서버에는 OpenSSL 모듈이 기본으로 설치되어 있습니다.)
- 윈도우 환경에서 이용하실 경우 윈도우+PHP+OpenSSL 자체의 버그로 인해서 php 5.4 이상을 사용하셔야 합니다. 리눅스(웹호스팅)에서는 PHP 5.3 이상이면 무방합니다.
- JS를 해석 할 수 있는 지능화된 고성능 스팸봇은 및 사람이 직접 올리는 스팸은 차단 할 수 없습니다.
    - 지능화된 스팸봇은 CAPTCHA 이외에는 스팸을 차단 할 수 없으며, 사람이 올리는 스팸은 어느것으로도 차단할 수 없습니다.
    - 다만 경험상 경제적인 문제(효율성) 때문인지 지능화된 고성능 스팸봇은 거의 없습니다. 이걸 뚦는것을 본적이 없네요.
사진 : http://jotarun.deviantart.com/art/Android-212204119


### V1.0.4로부터  변경내역
- 쪽지발송 스팸까지 차단하도록 개선
- 기타 xe captcha에 포함된 act까지 전부 검증.
