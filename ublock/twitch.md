Current Twitch rules
---------------------

```
!!! Twitch

!! Enable when needed.  They keep rotating functions and you're too lazy to find something better
! twitch.tv##+js(setTimeout-defuser.js)
! twitch.tv##+js(setTimeout-logger.js)
! static-cdn.jtvnw.net##+js(setTimeout-logger.js)

static-cdn.jtvnw.net##+js(stif)



@@||pubsub-edge.twitch.tv/v1$websocket,domain=www.twitch.tv
@@||irc-ws.chat.twitch.tv^$websocket,domain=www.twitch.tv

!!  Graphic sql..  part of their new API
@@||gql.twitch.tv/gql$xhr,domain=www.twitch.tv

@@||static.twitchcdn.net/config/manifest.json?v=1$xhr,domain=twitch.tv


@@||www.twitch.tv/directory/*$inline-script,domain=www.twitch.tv

@@||video-edge-*.pdx01.abs.hls.ttvnw.net/v1/*$xhr,domain=twitch.tv

@@||d2nvs31859zcd8.cloudfront.net/*/storyboards/*$xhr,domain=twitch.tv

! And so it begins.. wtf.
! WebASM slows at least Firefox down
! https://static.twitchcdn.net/assets/wasmworker.min-2ed166ab01108ed09e04.wasm
||static.twitchcdn.net/assets/wasmworker.min-*.wasm$xhr,domain=www.twitch.tv
||static.twitchcdn.net/assets/wasmworker.min-*.wasm$xhr,domain=static.twitchcdn.net

! New as of April  2020 ish
! https://app.link/_r?sdk=web2.53.2&branch_key=key_live_jgBdao5vVtyZ3kappaforsenooQltZ&callback=branch_callback__16
||app.link/_r?*

! 5/24/2020 twitch.tv  Needed for their helpsite
@@||e26428.dscx.akamaiedge.net^$xhr,domain=help.twitch.tv

! ||s.amazon-adsystem.com/iu3?pid=49002271-48b6-4ccb-bf4c-f82acb404220$subdocument,domain=twitch.tv
||s.amazon-adsystem.com/iu3?pid=*$subdocument,domain=twitch.tv

||s.amazon-adsystem.com^$image,domain=www.twitch.tv
||cdn.branch.io^$script,domain=www.twitch.tv
||sentinel.twitchsvc.net/error-report

!! Stupid things their devs do
||www.twitch.tv/experiments.json

||static-f.twitchcdn.net/assets/obs_logors_1x-ea09acc52659eb5399b6.png$image

!! Moar analytics.. they rotate this for some reason
||client-event-reporter.twitch.tv/v1/stats$xhr,domain=www.twitch.tv,important
||client-event-reporter.twitch.tv/$xhr,domain=twitch.tv,important
||client-event-reporter.twitch.tv^$important


! https://countess.twitch.tv/ping.gif?u=%7B%22id%22%3A%22540998998%22%2C%22type%22%3A%22vod%22%7D"
||countess.twitch.tv^$important

! Globaly blocked
! ||www.gstatic.com/cv/js/sender/v1/cast_sender.js?loadCastFramework=1$script,important


!!  Fake video chunk server
||video-edge-de8de7.pdx01.abs.hls.ttvnw.net/v1/segment/*$xhr,domain=twitch.tv,important


! Much of their site is hosted on fastly under sni
@@||twitch.map.fastly.net^$xhr,domain=twitch.tv
||static.twitchcdn.net/assets/sentry-*.js$script,domain=twitch.tv,important

! Amazon Video Ads SDK
! https://d2v02itv0y9u9t.cloudfront.net/dist/1.0.3/v6s.js  
||d2v02itv0y9u9t.cloudfront.net^$domain=twitch.tv,important

! Global block
! ||cdn-gl.imrworldwide.com^$important
||countess.twitch.tv/ping.gif$image,1p,important


!! Unfuck  their interface changes
www.twitch.tv##.tw-relative.tw-justify-content-center.tw-flex.tw-align-items-center.featured-content-carousel
www.twitch.tv##div .tw-media-card-meta__links > div:nth-of-type(2) > .tw-ellipsis.tw-c-text-alt-2 > .tw-link--inherit.tw-link--hover-underline-none.tw-link.tw-interactive:contains(VALORANT):nth-ancestor(11)

! www.twitch.tv##.side-nav__scrollable_content.simplebar-content
! www.twitch.tv##.scrollable-area--suppress-scroll-x.scrollable-area.tw-flex-grow-1 > .simplebar-scroll-content


! www.twitch.tv##.scrollable-area--suppress-scroll-x.scrollable-area.tw-flex-grow-1
! www.twitch.tv##.tw-z-above.tw-full-height.tw-flex-shrink-0.tw-c-background-alt.side-nav > .tw-full-height
www.twitch.tv##.tw-z-above.tw-full-height.tw-flex-shrink-0.tw-c-background-alt.side-nav
www.twitch.tv##.tw-relative.prime-offers

dashboard.twitch.tv##tw-absolute.sunlight-onboarding-welcome__video
dashboard.twitch.tv##sunlight-onboarding-welcome__image-background
dashboard.twitch.tv##.tw-pd-y-4.tw-pd-x-3.tw-justify-content-center.tw-flex-shrink-0.tw-flex-grow-1.tw-flex-column.tw-flex.tw-align-center
dashboard.twitch.tv##.tw-full-height.tw-flex-shrink-1.tw-flex-grow-1.tw-flex-column.tw-flex.tw-align-items-stretch
dashboard.twitch.tv##.sunlight-modal__backdrop.ReactModal__Overlay--after-open.ReactModal__Overlay


!!! - Twitch
```
