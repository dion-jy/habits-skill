# habits-skill

AI agent skill for [HabitLoop](https://github.com/dion-jy/uhabits) — read/write habit data.

## Setup (one-time)

1. Open the app → Settings → Sign in with Google
2. Settings → Link Agent → copy the code
3. Run:
```bash
python3 habits link <paste-code-here>
```

No API keys or credentials needed.

## Commands

```bash
python3 habits list              # List habits
python3 habits summary           # Streak & completion stats  
python3 habits entries --days 7  # Recent entries
python3 habits check <name> YES  # Check a habit
python3 habits check <name> NO   # Uncheck
python3 habits status            # App vs DB sync status
python3 habits coach "message"   # Send coaching notification
python3 habits whoami            # Show linked info
```

## How it works

1. App syncs habit data to Supabase in real-time
2. This skill accesses Supabase via the agent code (RLS enforced)
3. No admin keys — each user's data is isolated
