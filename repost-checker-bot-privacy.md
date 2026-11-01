# Privacy policy: Repost Checker

*Last updated: 2026-11-01. Host this page at a public address and save that address in the app's details in the
Reddit developer portal.*

**Who we are.** Repost Checker ("the app") is a Reddit moderation app by u/kei-kazuki. Contact: message that user on
Reddit.

## What the app stores

Everything is stored in the app's private storage for **one community only**. One community can never see another's
data, and the app has no server of its own.

| Data | Why | How long |
| --- | --- | --- |
| A fingerprint of each post's image (a 16-character code, not the image), the post id and the post time | To recognise reposts | Until the post is deleted by its author or taken down by Reddit, or the moderators' retention limit. A post a moderator removed is kept unless the moderators chose to forget removed posts |
| The author's username as seen at submission | To recognise someone reposting their own post | 30 days by default (moderators may choose 1-90), then erased; the fingerprint stays |
| If "edited copies" matching is on: short codes and positions of small patches of the picture (no pixels) | To recognise edited copies | Same as the fingerprint; oldest dropped above a cap |
| If AI detection is on: the score of each checked post | To show the result and avoid paid re-checks | 30 days |
| If repeat-reposter strikes are on: a user's lowercase username and the ids of their recent reposts | To count reposts | The strike window set by the moderators (30 days by default, 90 at most) |
| If the "is this a repost?" command is on: a per-user daily request counter | To limit requests | 2 days |
| A moderator's blacklist entry: the fingerprint, the post id, the reason the moderator typed and the time (not the moderator's name) | To remove reposts of an image the moderators blacklisted | Until the moderators remove it or the post is deleted by its author or Reddit |
| Counters, and a short log of recent events and errors (which can name a user) | To show the status and activity report | Logs 30 days; daily counters 40 days; lifetime totals are only numbers |
| API keys the moderators typed into the AI detection settings | To call the service | Until the moderators clear the fields. They are installation settings, so every moderator of that community can read them |

**Not stored:** pictures, titles, links and comment text. They are read from Reddit when needed (for example to
write a table of earlier posts) and are not kept.

## Deletion

* **A post is deleted** (by its author or by Reddit): the fingerprint, local-feature points, stored author, AI score
  and the link to the bot's comment are erased immediately, including a blacklist entry for it.
* **A post is deleted before the app has seen it:** nothing is saved. An image that can no longer be loaded is not
  saved either.
* **A moderator removes a post:** it stays remembered and is shown as removed in a table, unless the moderators turned
  on "Forget posts removed by moderators" (then it is forgotten, except a blacklist entry they made).
* **A user's account is deleted:** the stored name disappears when its retention period ends (30 days by default,
  90 at most).
* **The app is uninstalled:** all data of that community is deleted.

## What leaves Reddit

* The app downloads images and previews **from Reddit's own image servers** (`i.redd.it`, `preview.redd.it`,
  `external-preview.redd.it`). Nothing is sent to them except the request for the image.
* **Only if the moderators turn on AI detection and enter their own key:** for a checked post, SightEngine
  (`api.sightengine.com`) receives the public image address and Google Gemini (`generativelanguage.googleapis.com`)
  receives the image, together with the moderators' own key. The moderators choose which one is used. They process it
  under their own terms and privacy policies. The app does not send any username, post text or other data to them
  and does not use Reddit data to train any model.
* **Reverse-search links** (optional) are only links; following one is the reader's choice.
* RedGifs, Imgur and similar clips are recognised by the id in their address; their servers are not contacted.

## What the app does not do

It does not sell or share data, does not build profiles of people, does not track or surveil users, does not collect
passwords or personal information, and does not analyse faces or any biometric data.

## Your choices

Moderators control every feature in the app settings and can uninstall at any time. Redditors can delete their posts
(see *Deletion*) or contact the developer to ask what is stored.

## Contact

Questions about this policy: message u/kei-kazuki on Reddit.
