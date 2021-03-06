---
layout: page
title: Feeds

---

### News & Reviews

Sometimes there is a newsworthy item (submissions welcome!) or client release and details get posted on the blog: <https://f-droid.org/news-and-reviews>. In the past we had reviews of apps with screenshots and it would be great to have more; and who knows they might make their way into the client some day!

### Builds

Find out exactly when apks are available or when descriptions change: <https://f-droid.org/wiki/api.php?action=feedcontributions&user=Robot>. The status of the most recent build for an app can be obtained by appending /lastbuild to the wiki url of the package. Builds happen a couple of times a day ; a new repo index is only published once all outstanding builds are finished.

### Source Code

If you have an account on GitLab you can watch the F-Droid repos, or subscribe to atom feeds for them. A feed including actions from all fdroid repositories is available at <https://gitlab.com/fdroid.atom>.

### Forums

You can subscribe to new [forum](https://forum.f-droid.org/) posts and threads via the following URLs:

- <https://forum.f-droid.org/posts.rss>
- <https://forum.f-droid.org/latest.rss>

### Wiki

The human changes to the wiki: <https://f-droid.org/wiki/index.php?title=Special:RecentChanges>

### Bugs and Suggestions

<https://gitlab.com/fdroid/fdroidclient/issues>, <https://gitlab.com/fdroid/fdroidserver/issues>, <https://gitlab.com/fdroid/fdroiddata/issues>: All expose RSS feeds, and also email notifications if desired.

### IRC

chat.freenode.net #fdroid or #fdroid-dev. The channels are logged at <https://botbot.me/freenode/fdroid/> and <https://botbot.me/freenode/fdroid-dev/>.

## OPML import to a feed reader

For importing into your favourite news reader, save the following text as feeds.opml and add/remove feeds your are interested in.

On Android we have [de.shandschuh.sparserss](https://f-droid.org/repository/browse/?fdfilter=de.shandschuh.sparserss&fdid=de.shandschuh.sparserss), [net.fred.feedex](https://f-droid.org/repository/browse/?fdfilter=net.fred.feedex&fdid=net.fred.feedex), [de.danoeh.antennapod](https://f-droid.org/repository/browse/?fdfilter=de.danoeh.antennapod&fdid=de.danoeh.antennapod), [org.ttrssreader](https://f-droid.org/repository/browse/?fdfilter=org.ttrssreader&fdid=org.ttrssreader) (requires a tt-rss server to connect to) and [com.newsblur](https://f-droid.org/repository/browse/?fdfilter=com.newsblur&fdid=com.newsblur) (via newsblur.com). On the desktop you could use the Akregator for KDE, Liferea for Gnome or [http://newsbeuter.org newsbeuter] which is nice if you like working in a terminal.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<opml version="1.0">
  <head>
    <title>F-Droid related feeds</title>
  </head>
  <body>
    <outline title="F-Droid">
      <outline type="rss" title="News and Reviews" xmlUrl="https://f-droid.org/feed" htmlUrl="https://f-droid.org/news-and-reviews/"/>
      <outline type="rss" title="Wiki Changes by Humans" xmlUrl="https://f-droid.org/wiki/index.php?title=Special:RecentChanges&amp;feed=atom" htmlUrl="https://f-droid.org/wiki/page/Special:RecentChanges"/>
      <outline type="rss" title="Latest Builds" xmlUrl="https://f-droid.org/wiki/api.php?action=feedcontributions&amp;user=Robot&amp;feedformat=atom" htmlUrl="https://f-droid.org/wiki/page/Special:Contributions/Robot"/>
    </outline>
  </body>
</opml>
```
