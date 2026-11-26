# 학습 결과 확인

학습 결과(웹 주소·이미지·글)를 칸마다 넣으면, QR로 접속해 **분할 화면**으로 볼 수 있는 주소를 만들어 주는 정적 웹 페이지입니다.
입력한 내용은 서버에 저장되지 않고 주소(`#d=…`) 안에만 담깁니다.

## 사용한 오픈 소스 (MIT)

- [Split.js](https://github.com/nathancahill/split) 1.6.5 — 분할 화면 크기 조절
- [qrcode-generator](https://github.com/kazuhikoarase/qrcode-generator) 2.0.4 — QR 코드 생성
- [lz-string](https://github.com/pieroxy/lz-string) 1.5.0 — 주소 압축
