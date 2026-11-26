# Marvin

Marvin is a habit tracker website that helps you build good habits and track your growth.

Live site: https://wayneliberty33-dotcom.github.io/Marvin/

## What it does
- Create an account and log in (with a "Forgot password?" reset by email)
- Add a habit, tick it done for today, delete it
- See your current streak (days in a row), best streak and total days
- See the last 7 days at a glance
- A reminder banner shows how many habits are left to tick today (for example "1 habit left today"),
  warns you when a streak is at risk, and turns green when everything is done
- Your habits are saved to your account, so they appear on any device
- Each person can only see their own habits

## How it is built
- `index.html` is the whole website (page, look and code in one file)
- Supabase provides the database and the login
  - tables: `habits` and `check_ins`
  - Row Level Security rules make sure people only access their own rows

## Safety notes
- Passwords are handled by Supabase. They are never stored in this project.
- This project only contains the public (publishable) Supabase key.
  Never add a secret or service_role key to this repository.
