# 라이브 스코어보드 (중계 오버레이)

OBS 브라우저 소스 · 카메라파이 웹 오버레이에 그대로 얹어 쓰는 점수판.
HTML 한 파일이라 설치·빌드가 없다.

- 조작   https://today119.github.io/scoreboard/?view=control
- 오버레이 https://today119.github.io/scoreboard/?view=overlay&pos=BL&scale=1

주소 옵션
- `view=overlay|control`
- `pos=TL|TC|TR|BL|BC|BR` 오버레이 위치
- `scale=0.5~2` 크기

디자인 출처: AI Studio 「LiveStream Overlay Pro」의 `components/OverlayView.tsx`.
영상편집·통계차트·AI 중계멘트·motion 은 중계에 불필요해 걷어냈다.
