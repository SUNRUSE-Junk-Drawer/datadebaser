# Datadebaser

## What's the big idea?

According to the [SQLite documentation](https://www.sqlite.org/faq.html#q19), "SQLite will easily do 50,000 or more INSERT statements per second on an average desktop computer".

Hmm.  At 60FPS, that's 833.3 recurring queries per frame.

- You've got tables for state and data.
- You've got views for "rendering".
- You've got `INSTEAD OF` triggers for making changes to state in response to event handlers.

Can you make a *realtime action game* almost entirely in SQLite?
