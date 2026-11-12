# Aphasia-communication-tool-in-inpatient-care
Using Python the goal of this repo is to **Build the smallest useful prototype.** A tablet web app with:
   - a core hospital board (pain, toilet, thirst, positioning, yes/no, "I don't understand", family)
   - a short profile (family names, a few interests, preferred phrases)
   - a suggestion row ranked by context and past selections
   Logging what was offered, chosen, and rejected from day one.

aphasia-aac/
  app/
    main.py          # FastAPI routes
    ranking.py       # scores candidate phrases from context + history
    profile.py       # patient profile (names, preferences, access settings)
    db.py            # SQLite logging: offered / chosen / rejected
  data/
    core_board.json  # hospital core vocabulary
  static/            # HTML, CSS, JS for the tablet
  tests/
