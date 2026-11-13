# Production uptime

GitHub Actions checks the public production page and API health route on a five-minute schedule. No LLM calls or credentials are used. The endpoint URLs are repository secrets. Failed runs notify the GitHub account that owns the schedule when Actions failure emails are enabled.

GitHub may delay or drop scheduled runs, and public-repository schedules can be disabled after 60 days without repository activity. Check the Actions history regularly; this is best-effort monitoring.
