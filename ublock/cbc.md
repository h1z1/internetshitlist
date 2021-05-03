CBC (Canadian Broadcasting Corporation)
--------------------------------------

Long overdue this site got reeeled in.  The amount of tracking on it is retarded for being a national broadcaster

It changed post covid.  They take an extremely agressive posture against the public.

uMatrix is technically "deprecated" though still preferred..

```
!- CBC
!- CBC Canadian Broadcasting Corporation, aka Canadian Propaganda Network
!- CBC

! -- uMatrix

www.cbc.ca www.cbc.ca doc allow
i.cbc.ca i.cbc.ca doc allow
i.cbc.ca i.cbc.ca image allow

www.cbc.ca cbc.ca css allow
www.cbc.ca cbc.ca image allow
www.cbc.ca cbc.ca media allow
www.cbc.ca www.cbc.ca css allow
www.cbc.ca www.cbc.ca image allow
www.cbc.ca www.cbc.ca media allow
www.cbc.ca www.cbc.ca xhr allow
www.cbc.ca i.cbc.ca css allow
www.cbc.ca i.cbc.ca image allow
www.cbc.ca i.cbc.ca media allow
www.cbc.ca i.cbc.ca script allow

www.cbc.ca adlightning.com * block
www.cbc.ca cdn-cbc-v3.conductrics.com * block
www.cbc.ca cdn.viafoura.net * block
www.cbc.ca chartbeat.com * block
www.cbc.ca conductrics.com * block
www.cbc.ca crwdcntrl.net * block
www.cbc.ca cxense.com * block
www.cbc.ca data.cbc.ca * block
www.cbc.ca go-mpulse.net * block
www.cbc.ca indexww.com * block
www.cbc.ca ingest.sentry.io * block
www.cbc.ca js-sec.indexww.com * block
www.cbc.ca moatads.com * block
www.cbc.ca s.go-mpulse.net * block
www.cbc.ca scdn.cxense.com * block
www.cbc.ca scorecardresearch.com * block
www.cbc.ca sentry.io * block
www.cbc.ca sombersurprise.com * block
www.cbc.ca static.chartbeat.com * block
www.cbc.ca uie.data.cbc.ca * block
www.cbc.ca us-central1-digitalproducts-gabbo.cloudfunctions.net * block
www.cbc.ca viafoura.net * block
www.cbc.ca z.moatads.com * block


!
!-- uBlock
!
||www.cbc.ca/akam/11/*$script,1p
||www.cbc.ca/a/scripts/ErrorPage.ca*.js$script,1p
||www.cbc.ca/g/stats/js/ads.js$script,1p
||www.cbc.ca/g/stats/comscore.json$xhr
||www.cbc.ca/g/stats/js/cbc-stats-bottom.js$1p
||www.cbc.ca/g/stats/js/cbc-stats-top.js$1p
||www.cbc.ca/g/stats/comscore.json$xhr
||www.cbc.ca/g/stats/*$script,1p
||www.cbc.ca/g/stats/*$script,1p,important
||www.cbc.ca/ads/*$script,1p
||uie.data.cbc.ca^$xhr,1p
www.cbc.ca##.privacyNotification

! ||ups.data.cbc.ca/v0/UIEUser//UPSPreferences/xxxxx$xhr,domain=www.cbc.ca,important
||ups.data.cbc.ca/v0/UIEUser$xhr,domain=www.cbc.ca,important
||www.cbc.ca/i/caffeine/$document,domain=www.cbc.ca,important

||cdn-cbc-v3.conductrics.com^$script,domain=cbc.ca


||js-sec.indexww.com/ht/p/*.js$script,domain=cbc.ca
||cdn.viafoura.net^$domain=cbc.ca

||sombersurprise.com/v2/0/*$domain=cbc.ca
||dpm.demdex.net/id?*
||ad.crwdcntrl.net^$script

||scdn.cxense.com^$domain=cbc.ca
||static.chartbeat.com^$script,domain=cbc.ca
||imasdk.googleapis.com/js/sdkloader/ima3.js$script,domain=cbc.ca
||e4518.dscx.akamaiedge.net^$domain=cbc.ca
||s.go-mpulse.net^$script
||connect.facebook.net/en_US/fbevents.js$script,domain=cbc.ca
||tags.crwdcntrl.net^$domain=cbc.ca


||z.moatads.com^$script,domain=cbc.ca


! --- CBC

```
