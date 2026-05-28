# HabitLoop Skill

습관 데이터를 읽고 쓰는 agent skill.

## Setup

`.env.example`을 `.env`로 복사하고 credentials 입력. 그 후 `python3 habits link`로 사용자 연결.

## 사용자가 습관 관련 요청 시

- "내 습관 확인해줘" → `python3 habits summary`
- "오늘 운동 체크해" → `python3 habits check exercise YES`
- "최근 기록 보여줘" → `python3 habits entries`
- "앱 상태 어때" → `python3 habits status`
