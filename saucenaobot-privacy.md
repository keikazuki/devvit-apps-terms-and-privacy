# SauceNaoBot Privacy Policy

DRAFT, not legal advice. Replace `[CONTACT]` and host this at a public URL.
Last updated: 2026-10-30

**Summary:** SauceNaoBot does not collect personal data, does not use analytics
or advertising, and does not sell or share data. It only handles what it needs
to look up one post at a time.

## What the app handles

| Data                                                              | Why                                                                   | Where it goes                                                                                          | How long                                           |
| ----------------------------------------------------------------- | --------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------ | -------------------------------------------------- |
| Post ID                                                           | To queue the post, avoid answering it twice, and retry failed lookups | Reddit-provided app storage                                                                            | See "Retention"                                    |
| Post image URL                                                    | To look up the image                                                  | Sent (URL only) to saucenao.com; read from Reddit when needed, not stored by the app                   | Not stored                                         |
| SauceNAO API key entered by moderators                            | To authenticate lookups                                               | Stored in the app's Reddit-provided settings for that subreddit; sent to saucenao.com with each lookup | Until a moderator removes it or uninstalls the app |
| Flair template IDs and comment text options entered by moderators | App configuration                                                     | App settings                                                                                           | Until changed or uninstalled                       |
| A daily-limit cooldown marker                                     | To stop calling SauceNAO after it reports its limit                   | Reddit-provided app storage                                                                            | Expires automatically                              |

## What the app does not do

- It does not store post titles, post bodies, comments, or usernames beyond what
  Reddit itself keeps (the reply mentions the post author's username, as the
  original bot did, but the app does not save it).
- It does not collect browsing data, IP addresses, or device information.
- It does not send any Reddit user information to SauceNAO. Only the image URL
  and the moderators' API key are sent.

## Third parties

- **SauceNAO (saucenao.com)** receives the image URL and API key and is governed
  by its own privacy policy.
- **Reddit** hosts the app and its storage and is governed by Reddit's policies.

## Retention

All of this is post IDs and counters in the app's own Reddit-provided storage:

- the queue entry is deleted as soon as the post is processed (usually within a minute);
- a "seen" marker (to ignore duplicate notifications) expires after 7 days;
- an "answered" marker (so a post is never answered twice) expires after 30 days;
- a "moderator requested" marker expires after 2 days;
- a failed-download counter expires after 1 day;
- the daily-limit pause marker expires after at most 10 minutes;
- a running total of answered posts (one number, no post details), kept until the app is uninstalled.
  Uninstalling the app removes its stored data on Reddit's side.

## Security note for moderators

Reddit's per-subreddit text settings are not masked. Other moderators of the
subreddit who can open the app's settings can see the API key. Use a key you are
comfortable sharing with your mod team.

## Contact

[CONTACT]
