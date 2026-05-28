# HabitLoop Skill

습관 데이터를 읽고 쓰는 agent skill.

## 첫 사용 시

`.user` 파일이 없으면 사용자에게 앱에서 코드를 받아오라고 안내:
1. 앱 Settings → Sign in with Google
2. Settings → Link Agent → 코드 복사
3. `python3 habits link <코드>`

## 사용자가 습관 관련 요청 시

- "내 습관 확인해줘" → `python3 habits summary`
- "오늘 운동 체크해" → `python3 habits check exercise YES`
- "최근 기록 보여줘" → `python3 habits entries`
- "앱 상태 어때" → `python3 habits status`
