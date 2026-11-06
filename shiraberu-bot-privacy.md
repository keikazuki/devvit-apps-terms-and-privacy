# Shiraberu Privacy Policy

Last updated: 2026-11-06

**Summary:** Shiraberu does not use analytics or advertising and does not sell or share data. It
never stores the text of a comment. It keeps only what it needs to answer a comment once and to edit
or delete its reply later. Anything tied to a comment is removed after 30 days at the latest, or at
once when the comment is deleted. Statistics are off unless a community's moderators switch them on.

## What the app handles

| Data                                                                                                                                                            | Why                                                                      | Where it goes                                            | How long                                                                                                                                                                     |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ | -------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| The text of a comment that holds a request                                                                                                                      | To find the titles being requested                                       | Read from Reddit and used in memory; **not stored**      | Not stored                                                                                                                                                                   |
| The words between the brackets (the title as typed)                                                                                                             | To look the series up                                                    | Sent to AniList, Kitsu, VNDB or MangaUpdates (see below) | Not stored with the comment                                                                                                                                                  |
| The ID of the comment and of the app's reply, and a short fingerprint of the reply                                                                              | To avoid answering a comment twice and to edit or delete the reply later | Reddit-provided app storage for that subreddit           | 30 days, then removed automatically (or at once if the comment is deleted)                                                                                                   |
| Catalogue results (public information about a series)                                                                                                           | So that a popular title is not asked for again and again                 | Reddit-provided app storage for that subreddit           | Up to 30 days; anything cached because of a comment is erased when it is deleted                                                                                             |
| Statistics, **only if moderators switch them on**: how often each title was requested in the community, and each commenter's own requests (username and titles) | To answer `{!stats}` and `{!stats me}`                                   | Reddit-provided app storage for that subreddit           | Community totals until the app is uninstalled (no usernames, no comment text); a commenter's own numbers 30 days after their last request, and at once for a deleted comment |
| Aliases entered by moderators                                                                                                                                   | To answer nicknames correctly                                            | Reddit-provided app storage for that subreddit           | Until a moderator removes them                                                                                                                                               |
| Short-lived technical markers (processing and rate limits)                                                                                                      | To avoid duplicate work and runaway replies                              | Reddit-provided app storage for that subreddit           | Minutes to hours                                                                                                                                                             |

## What the app does not do

- It does not store comment text, post titles, or anything a person wrote.
- It does not send any Reddit user information (usernames, comment text, IP addresses) to any
  third-party site. Requests come from Reddit's servers and contain only the words that were
  between the brackets.
- It does not build profiles, rank people, or let anyone see another person's statistics.
- It does not collect browsing data or device information.

## Logs

The developer can read the app's logs. They contain comment IDs, counts and error messages, never
the text of a comment.

## Deleted and edited comments

If a user deletes the comment that made a request, the app deletes its own reply and erases what it
kept about that comment, including its counts in the statistics (if they are on) and anything cached
because of it. If the comment is edited, the reply is updated; if the edit removes every request, the
reply is deleted. If a user's account is deleted, nothing about that user remains after at most 30
days.

## Third parties

The app contacts only the public APIs of AniList (graphql.anilist.co), Kitsu (kitsu.io), VNDB
(api.vndb.org) and MangaUpdates (api.mangaupdates.com), only to look up a title a person wrote.
Each is governed by its own privacy policy. Other sites appear in replies only as links: the app
never contacts them. Reddit hosts the app and its storage and is governed by Reddit's policies.

## Contact

Message the moderators of r/SauceSharingCommunity through modmail
(https://www.reddit.com/message/compose?to=/r/SauceSharingCommunity).
