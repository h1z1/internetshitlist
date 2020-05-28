uBlock Rules for Reddit
------------------------

Because RES is a PITA

```

!!! Reddit

!! change to whatever.. overrides css on all subs
reddit.com#$#div.side{ background-color: black !important; }
reddit.com#$#body{ background-color: black !important; }
reddit.com#$#a.title{ background-color: lightgreen !important; }
reddit.com#$#*.md{ background-color: aquamarine !important; }


! reddit.com##+js(addEventListener-defuser.js )
! reddit.com##+js(addEventListener-defuser.js, click)


reddit.com##+js(addEventListener-defuser.js, pixelSuccess.gtm)
reddit.com##+js(addEventListener-defuser.js, pixelError.gtm)
reddit.com##+js(addEventListener-defuser.js, loaded.gtm)
reddit.com##+js(addEventListener-defuser.js, onshow)


! Their retarded trampoline links
reddit.com##+js(aopr, r.utils.replaceUrlParams)


reddit.com##+js(addEventListener-defuser.js, focus)
reddit.com##+js(addEventListener-defuser.js, mouseover)
reddit.com##+js(addEventListener-defuser.js, mousedown)
reddit.com##+js(addEventListener-defuser.js, mouseout)
reddit.com##+js(addEventListener-defuser.js, keypress)

||old.reddit.com/web/*$xhr,domain=old.reddit.com
||old.reddit.com/chat/minimize$subdocument,1p,important
||reddit.com/static/pixel.png$image
||reddit.com/static/pixel.png$image,domain=old.reddit.com,important
||www.redditstatic.com^$script,domain=reddit.com

@@||reddit.map.fastly.net^$xhr,domain=mod.reddit.com

@@||www.redditstatic.com^$script,domain=reddit.com
@@||www.redditstatic.com^$image,domain=reddit.com
@@||www.redditstatic.com^$stylesheet,domain=reddit.com

@@||*.thumbs.redditmedia.com^$stylesheet,domain=reddit.com

@@||*.thumbs.redditmedia.com/_CFJQXtRrNafCUqmMwc_vIHYMic0VmLLWC7RuPoNFw4.png$image,domain=reddit.com

!! added otherwise posting fails entirely
@@||reddit.map.fastly.net^$xhr,domain=old.reddit.com


||a.thumbs.redditmedia.com/IVdlVkLeR6bvnNY3hWzLcwYtRgq7JN_skVzSYoz-Sq8.png$image
||a.thumbs.redditmedia.com/j-NSfkp2XMEmjOdR0uAmZmYmYAKSgL7Nz4Lpu7lWbo8.png$image
||b.thumbs.redditmedia.com/n_9RRLmpt1R8Pb6FUSakAGIolr18bHzmzxWa6qGH8CE.png$image
||b.thumbs.redditmedia.com/Q6hoCcTH0JBkq-cceSij_y89g1NunS1MfSN5ac30OqE.png$image

||www.redditmedia.com/gtm/*$subdocument,domain=reddit.com,important

!! Unfuck UI
reddit.com##.promotedlink
reddit.com##.premium-banner

reddit.com##[id^="CommentAwardBadges--"]

reddit.com###mail
reddit.com###ad_2

reddit.com##.happening-now
reddit.com##.commentsignupbar__textarea
reddit.com##.commentsignupbar__container

reddit.com##.hohoho.sidebox
reddit.com##.listingsignupbar.infobar
reddit.com###header-bottom-left

reddit.com###pinnable-content-e7vt6s
reddit.com###pinnable-content-dylzpv
reddit.com###pinnable-content-dz91wj

reddit.com###thing_t3_dymrkg > .unvoted.entry
reddit.com###thing_t3_dine1y > .unvoted.entry
reddit.com###thing_t3_dmnu6l > .unvoted.entry


! Block by title
reddit.com## .top-matter > .title:contains(Greek):nth-ancestor(3),important
reddit.com## .top-matter > .title:contains(Sodapoppin):nth-ancestor(3),important
reddit.com## .top-matter > .title:contains(Mizkif):nth-ancestor(3),important
reddit.com## .top-matter > .title:contains(Mitch Jones):nth-ancestor(3),important
reddit.com## .top-matter > .title:contains(OfflineTV):nth-ancestor(3),important
reddit.com## .top-matter > .title:contains(Trainwreckstv):nth-ancestor(3),important

! Block by author
reddit.com##div[data-author*="Normiesreeee69"],important

! Block by flair/tag
reddit.com##div[data-permalink*="alinity"],important
reddit.com##div[data-permalink*="train"],important
reddit.com##div[data-permalink*="offlinetv"],important
reddit.com##div[data-permalink*="destiny"],important
reddit.com##div[data-permalink*="Greek"],important
reddit.com##div[data-permalink*="Mitch Jones"],important

! Block comments by author
reddit.com## .unvoted.entry > .top-matter > .tagline > span:contains(Cmac0801)
reddit.com## .unvoted.entry > .top-matter > .tagline > span:contains(baekovsky1812)

! Block post by sub (cleans up r/all)
reddit.com## .unvoted.entry > .top-matter > .big-tagline.tagline > .may-blank.hover.subreddit:contains(r/cock):nth-ancestor(4),important
reddit.com## .unvoted.entry > .top-matter > .big-tagline.tagline > .may-blank.hover.subreddit:contains(r/Sissies):nth-ancestor(4),important
reddit.com## .unvoted.entry > .top-matter > .big-tagline.tagline > .may-blank.hover.subreddit:contains(r/GaySnapchat):nth-ancestor(4),important
reddit.com## .unvoted.entry > .top-matter > .big-tagline.tagline > .may-blank.hover.subreddit:contains(r/sissydressing):nth-ancestor(4),important
reddit.com## .unvoted.entry > .top-matter > .big-tagline.tagline > .may-blank.hover.subreddit:contains(r/Sissy_hot):nth-ancestor(4),important
reddit.com## .unvoted.entry > .top-matter > .big-tagline.tagline > .may-blank.hover.subreddit:contains(r/Cock):nth-ancestor(4),important
reddit.com## .unvoted.entry > .top-matter > .big-tagline.tagline > .may-blank.hover.subreddit:contains(r/MassiveCock):nth-ancestor(4),important
reddit.com## .unvoted.entry > .top-matter > .big-tagline.tagline > .may-blank.hover.subreddit:contains(r/onlyfanspromo):nth-ancestor(4),important

!!! - Reddit
