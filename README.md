# 학습 결과 확인

학습 결과(웹 주소·이미지·글)를 칸마다 넣으면, QR로 접속해 **분할 화면**으로 볼 수 있는 주소를 만들어 주는 정적 웹 페이지입니다.
참여 인원(최대 30명)에 맞춰 칸 수가 자동으로 나뉘고, 각 칸은 누르면 확대·축소됩니다.
입력한 내용은 서버에 저장되지 않고 주소(`#d=…`) 안에만 담깁니다.

## 실시간 방

교사가 방을 만들고 QR을 띄우면 학생이 각자 접속해 자기 웹 학습 결과(주소·글)를 올리고, 모두의 분할 화면에 바로 나타납니다.
통신은 공개 MQTT 중계 서버(broker.emqx.io)를 거치며, 방 상태는 접속한 기기들끼리 맞추고 각 기기의 브라우저에 저장합니다.

## 사용한 오픈 소스 (MIT)

- [Split.js](https://github.com/nathancahill/split) 1.6.5 — 분할 화면 크기 조절
- [qrcode-generator](https://github.com/kazuhikoarase/qrcode-generator) 2.0.4 — QR 코드 생성
- [lz-string](https://github.com/pieroxy/lz-string) 1.5.0 — 주소 압축
- [SortableJS](https://github.com/SortableJS/Sortable) 1.15.7 — 칸 순서 끌어 바꾸기
- [Panzoom](https://github.com/timmywil/panzoom) 4.6.2 — 이미지 확대·축소
- [MQTT.js](https://github.com/mqttjs/MQTT.js) 5.16.1 — 실시간 방(학생이 직접 올리기) 통신
