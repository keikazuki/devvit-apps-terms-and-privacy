# Shiraberu Privacy Policy

Last updated: 2026-11-06

**Summary:** Shiraberu does not use analytics or advertising and does not sell or share data. It
never stores the text of a comment. It keeps the minimum it needs to answer one comment, to edit or
delete its reply later, and to show a community's statistics, and everything that is tied to a
person or to a comment is removed after 30 days at the latest, or at once when the comment is
deleted.

## What the app handles

| Data                                                                                                                                                | Why                                                                                                                                                      | Where it goes                                            | How long                                                                                                                                            |
| --------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------- |
| The text of a comment that holds a request (and nothing else about the comment)                                                                     | To find the titles being requested                                                                                                                       | Read from Reddit and parsed in memory; **not stored**    | Not stored                                                                                                                                          |
| The words between the brackets (the title as typed)                                                                                                 | To look the series up                                                                                                                                    | Sent to AniList, Kitsu, VNDB or MangaUpdates (see below) | Not stored with the comment (see the cache row)                                                                                                     |
| Comment ID, the ID of the app's reply, a digest of the reply text, the catalogue titles the comment was answered with, and the commenter's username | To avoid answering a comment twice, to edit or delete the reply later, and to take the comment's counts out of the statistics if it is edited or deleted | Reddit-provided app storage (Redis) for that subreddit   | 30 days, then removed automatically (or at once if the comment or reply is deleted)                                                                 |
| The commenter's own statistics: their username and the titles they requested, with counts                                                           | Only to answer `{!stats me}` for that person                                                                                                             | Reddit-provided app storage for that subreddit           | 30 days after their last request (the key expires automatically); removed at once for a deleted comment                                             |
| The community's statistics: how many times each catalogue title was requested, totals, a running sum for the average                                | To answer `{!stats}` and the "Stats" line of the long form                                                                                               | Reddit-provided app storage for that subreddit           | Until the app is uninstalled; contains no usernames and no comment text                                                                             |
| Which catalogue entries a search matched (their ids), stored under a one-way hash of the searched words                                             | To answer a title that is asked for again and again without asking the catalogue again                                                                   | Reddit-provided app storage for that subreddit           | Up to 30 days (1 hour when nothing was found); removed at once when the comment that made the search is deleted                                     |
| Public catalogue entries (title, genres, description, links, the ids of the other databases)                                                        | The same                                                                                                                                                 | Reddit-provided app storage                              | A finished series up to 30 days; one still being published 2 days (1 day when not yet released); an airing anime 6 hours. Never longer than 30 days |
| Aliases entered by moderators (words, catalogue addresses)                                                                                          | To answer nicknames correctly                                                                                                                            | Reddit-provided app storage                              | Until a moderator removes them                                                                                                                      |
| A processing lock, an hourly reply counter, a "source is resting" marker                                                                            | To avoid duplicate work, cap the rate and spare the catalogues                                                                                           | Reddit-provided app storage                              | 5 minutes, 2 hours, and the time the catalogue asked for                                                                                            |

## What the app does not do

- It does not store comment text, post titles, or anything a person wrote except the catalogue titles
  listed above.
- It does not send any Reddit user information (usernames, comment text, IP addresses) to any
  third-party site. Requests come from Reddit's servers and contain only the words that were
  between the brackets.
- It does not build profiles, rank people, or let anyone see another person's statistics.
- It does not collect browsing data or device information.

## Deleted and edited comments

If a user deletes the comment that made a request, the app deletes its own reply and erases every
record it kept about that comment, including the comment's counts in the statistics, the
commenter's name, and the catalogue searches that were stored from the comment's words (the public
catalogue entries themselves belong to nobody and stay until they expire). If the comment is edited, the reply is updated and the counts follow the edit; if
the edit removes every request, the reply is deleted. If a user's account is deleted, nothing about
that user remains after at most 30 days.

## Third parties

The app contacts only the public APIs of AniList (graphql.anilist.co), Kitsu (kitsu.io), VNDB
(api.vndb.org) and MangaUpdates (api.mangaupdates.com), only to look up a title a person wrote.
Each is governed by its own privacy policy. Other sites (Anime-Planet, NovelUpdates, AniDB,
MyAnimeList and, if a moderator switches them on, Google, LiveChart, RanobeDB and MangaBaka) appear
in replies only as links: the app never contacts them. Reddit hosts the app and its storage and is
governed by Reddit's policies.

## Contact

Message the moderators of r/SauceSharingCommunity through modmail
(https://www.reddit.com/message/compose?to=/r/SauceSharingCommunity).
