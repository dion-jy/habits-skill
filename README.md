# habits-skill

AI agent skill for [HabitLoop](https://github.com/dion-jy/uhabits) — read/write habit data via Supabase.

## Setup

```bash
cp .env.example .env
# Fill in SUPABASE_URL and SUPABASE_SERVICE_ROLE_KEY
python3 habits link
# Enter the token in app: Settings → Link Agent
```

## Commands

```bash
python3 habits list              # List habits
python3 habits summary           # Streak & completion stats
python3 habits entries --days 7  # Recent entries
python3 habits check <name> YES  # Check a habit (partial name match)
python3 habits check <name> NO   # Uncheck
python3 habits status            # App vs DB sync status
python3 habits coach "message"   # Send coaching notification
python3 habits whoami            # Show linked user info
```

## How it works

1. App syncs habit data to Supabase in real-time
2. This skill reads/writes Supabase via REST API
3. User authentication via Google SSO + device linking token
4. All queries scoped to linked user (multi-user safe)
