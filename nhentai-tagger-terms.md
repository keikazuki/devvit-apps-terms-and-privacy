# nhentai-tagger Terms of Service

Last updated: 2026-11-03

nhentai-tagger ("the app") is a Reddit moderation helper for communities that share adult
artwork (hentai). When a user writes a gallery number or link in a comment, the app looks the
gallery up on a third-party site and replies with its title, page count and tags.

1. **Who may install it.** Moderators of a subreddit, using Reddit's Developer Platform. By
   installing you confirm you are authorised to configure the app for that community.
2. **Adult content.** The app is marked NSFW. It is intended only for communities that allow
   adult content, and moderators are responsible for installing it only where that is appropriate
   and permitted by Reddit's rules.
3. **How it is triggered.** The app acts only on comments that contain a request: a gallery
   number in the form `(123456)` or `}618395/0439fa3666{`, or `!tags` with a link. It does not
   browse, crawl or act on its own. It posts one reply per request as the app account, edits that
   reply if the request is edited, deletes it if the request comment is deleted, and, when a user
   replies `!link` to one of its replies, sends that user the links by private message. It looks
   galleries up through the public APIs of nHentai (nhentai.net) and E-Hentai (api.e-hentai.org).
4. **Galleries tagged loli or shota.** The app describes such a gallery like any other (title,
   page count, tags) but never makes it a hyperlink, neither in a reply nor in a `!link` message.
   Moderators can switch on "Hide the details of loli/shota galleries"; the app then only says
   "The gallery information is unavailable at this time." for them. Moderators decide whether this
   fits their community and Reddit's rules.
5. **Your own nHentai key (optional).** Moderators may enter their own nHentai API key in the
   app's settings. It is optional. You are responsible for the key and for staying within
   nHentai's own terms and limits. The app does not provide keys. Reddit does not mask this
   setting: other moderators of your subreddit can see it.
6. **Limits.** The app looks up at most 5 galleries per comment and posts at most 200 replies and
   100 private messages per hour per community.
7. **Accuracy.** Results are copied automatically from third-party sites. They can be wrong,
   incomplete, out of date or missing, and the app makes no guarantee about them.
8. **Third-party services.** Reddit, nHentai and E-Hentai have their own terms and may change or
   block access at any time. The app is not affiliated with or endorsed by any of them.
9. **No warranty, limited liability.** The app is provided "as is". To the extent the law allows,
   the developer is not liable for losses from its use or from downtime, errors, or removal of
   the app.
10. **Changes and removal.** The developer may change or discontinue the app. Moderators can
    uninstall it at any time.
11. **Contact.** Message the moderators of r/SauceSharingCommunity through modmail
    (https://www.reddit.com/message/compose?to=/r/SauceSharingCommunity).
