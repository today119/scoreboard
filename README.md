# 라이브 스코어보드 (중계 오버레이)

OBS 브라우저 소스 · 카메라파이 웹 오버레이에 그대로 얹어 쓰는 점수판.
HTML 한 파일이라 설치·빌드가 없다.

- 조작   https://today119.github.io/scoreboard/?view=control
- 오버레이 https://today119.github.io/scoreboard/?view=overlay&pos=BL&scale=1

주소 옵션
- `view=overlay|control`
- `pos=TL|TC|TR|BL|BC|BR` 오버레이 위치
- `scale=0.5~2` 크기
- `theme=dark|light` 점수판 색
- `layout=bar|corner|wide` 레이아웃 고정 (없으면 조작 화면에서 고른 것이 실시간으로 따라감)
- `room=코드` 다른 기기(폰)·OBS 와 실시간 연결

종목 (조작 화면 「경기 정보 → 종목」)
- 세트제: 배구(25점·마지막 15점) · 탁구(11점, 서브 2점마다 자동) · 배드민턴(21점·30점 상한) · 족구(15점) · 이스포츠
  → 목표 점수에 닿으면 「세트 종료」가 깜빡인다 (최종 점수를 보여준 뒤 사람이 누른다)
- 테니스 — 세트기록 | 게임 | 포인트. 0·15·30·40·AD, 노애드, 6:6 타이브레이크(7점), 서브 자동 교대
- 축구(전반·후반, 시간 올라감) · 농구(1Q~OT, +1·+2·+3, 팀파울·BONUS, 시간 내려감) · 줄넘기(ROUND, +1·+5·+10)
- 직접 설정 — 기간 이름·점수 버튼·세트제·서브·팀파울·목표점수를 골라 없는 종목도 만든다

디자인 출처: AI Studio 「LiveStream Overlay Pro」의 `components/OverlayView.tsx`.
영상편집·통계차트·AI 중계멘트·motion 은 중계에 불필요해 걷어냈다.
