# nhentai-tagger Privacy Policy

Last updated: 2026-11-03

**Summary:** nhentai-tagger does not collect personal data, does not use analytics or advertising,
and does not sell or share data. It handles only what it needs to answer one comment at a time,
and it never stores comment text or usernames.

## What the app handles

| Data                                                                                                                                | Why                                                                             | Where it goes                                                                       | How long                                                  |
| ----------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- | --------------------------------------------------------- |
| The text of a comment that asks for a lookup (and of its parent comment or post, for `!tags`)                                       | To find the gallery numbers and links being requested                           | Read from Reddit and parsed in memory; **not stored**                               | Not stored                                                |
| Comment ID, the ID of the app's reply, the gallery numbers requested (and whether each is tagged loli/shota, which is never linked) | To avoid answering a comment twice, and to edit, delete or link the reply later | Reddit-provided app storage (Redis) for that subreddit                              | 30 days, then removed automatically                       |
| The username of someone who replies `!link`                                                                                         | To send them the links by private message                                       | Used for that one message; **not stored**                                           | Not stored                                                |
| Copies of public gallery information (title, page count, tag names)                                                                 | To avoid asking the same site again and again                                   | Reddit-provided app storage for that subreddit                                      | Up to 30 days (reused for 7 by default)                   |
| A processing lock, an hourly reply counter, an hourly message counter, a "site is busy" pause marker, a "gallery not found" marker  | To avoid duplicate work, cap the rate and spare the sites                       | Reddit-provided app storage                                                         | 5 minutes, 2 hours, 2 hours, up to 10 minutes, 10 minutes |
| A marker that a comment's `!link` request was answered, and one that a reply already got its public `!link` answer                  | To answer each request once                                                     | Reddit-provided app storage                                                         | 30 days                                                   |
| Running totals (replies, galleries per site, link messages)                                                                         | Statistics shown to moderators                                                  | Reddit-provided app storage                                                         | Until the app is uninstalled                              |
| An optional nHentai API key entered by moderators                                                                                   | To raise the request limit                                                      | Stored in the app's Reddit-provided settings; sent only to nhentai.net, in a header | Until a moderator removes it or uninstalls the app        |
| The gallery number or token a user typed                                                                                            | To look the gallery up                                                          | Sent to nhentai.net or api.e-hentai.org (see below)                                 | Not stored by the app beyond the cache above              |

## What the app does not do

- It does not store comment text, post titles, or usernames. (The app compares a commenter's name
  with its own name and with the moderators' "users to ignore" list to avoid answering itself or
  other bots, and does not save it.)
- It does not send any Reddit user information (usernames, comment text, IP addresses) to any
  third-party site. Requests come from Reddit's servers.
- It does not collect browsing data or device information.

## Deleted comments

If a user deletes the comment that made a request, the app deletes its own reply and erases every
record it kept about that comment.

## Third parties

The app contacts only these sites' public APIs, only to look up the gallery a user asked for:
nhentai.net (nHentai) and api.e-hentai.org (E-Hentai). Each is governed by its own privacy policy.
Reddit hosts the app and its storage and is governed by Reddit's policies.

## Security note for moderators

Reddit's per-subreddit text settings are not masked. Other moderators of the subreddit who can open
the app's settings can see the API key you enter. Use a key you are comfortable sharing with your
mod team. It is optional.

## Contact

Message the moderators of r/SauceSharingCommunity through modmail
(https://www.reddit.com/message/compose?to=/r/SauceSharingCommunity).
