# Shiraberu Terms of Service

Last updated: 2026-11-05

Shiraberu ("the app") is a Reddit app for communities that talk about anime, manga, light novels
and visual novels. When a user writes the name of a series between brackets in a comment, the app
looks it up in public catalogues and replies with a short card: title, links, type, status,
number of episodes or volumes and genres.

1. **Who may install it.** Moderators of a subreddit, using Reddit's Developer Platform. By
   installing you confirm you are authorised to configure the app for that community.
2. **How it is triggered.** The app acts only on comments that contain a request: a title
   between brackets, such as `{Steins;Gate}`, `<Yotsuba to!>`, `]Overlord[` or `|Clannad|`, or
   `{!stats}`. It does not browse, crawl or act on its own. It posts one reply per comment
   that holds a request, as the app account, edits that reply if the request is edited and deletes it if the
   request comment is deleted. It looks titles up through the public APIs of AniList
   (graphql.anilist.co), Kitsu (kitsu.io), VNDB (api.vndb.org) and MangaUpdates
   (api.mangaupdates.com).
3. **Adult-rated titles.** The catalogues contain adult-rated works. By default the app skips them
   and a request for one gets no answer. Moderators of communities that allow adult content can
   switch on "Include adult-rated titles" in the settings; the app then answers such a request
   like any other (title, links, genres). Moderators decide whether this fits their community and
   Reddit's rules.
4. **Limits.** The app answers at most 30 requests per comment (moderators can lower this) and
   posts at most 200 replies per hour per community (moderators can change this).
5. **Accuracy.** Results are copied automatically from third-party catalogues and matched to the
   words a person typed. They can be wrong, incomplete, out of date or missing, and the app makes
   no guarantee about them. Moderators can pin a title to the right page with the alias tool.
6. **Statistics.** The app counts how often titles are requested in a community. A person can see
   their own numbers of the last 30 days with `{!stats me}`; nobody can see another person's.
7. **Third-party services.** Reddit, AniList, Kitsu, VNDB and MangaUpdates have their own terms
   and may change or block access at any time. The app is not affiliated with or endorsed by any
   of them, nor by Roboragi, whose request syntax and reply format it follows.
8. **No warranty, limited liability.** The app is provided "as is". To the extent the law allows,
   the developer is not liable for losses from its use or from downtime, errors, or removal of
   the app.
9. **Changes and removal.** The developer may change or discontinue the app. Moderators can
   uninstall it at any time.
10. **Contact.** Message the moderators of r/SauceSharingCommunity through modmail
    (https://www.reddit.com/message/compose?to=/r/SauceSharingCommunity).
