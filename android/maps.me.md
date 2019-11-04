Summary: Very common map application for android.  Based on OpenStreetMap
URL: https://maps.me

Though possibly the first application to offer offline maps, at the end of the day, avoid.  The telemetry is mindnuming.  

** At the very least use something like Android Firewall .. seriously regarless everyone should be running it **

- Both the company itself and their metrics (mail.ru) are heavily tied to Russian influence.  
- It is -not- possible to disable despite their claims.



Maps are downloaded over plain http

Other observed IPs | AS | Desc 
------------------ | --- | --------------------
217.69.139.134  | AS47764 | Mail.Ru Services  
185.205.76.32   | AS60476 | My.Com Services (mail.ru)
50.7.149.10     |         | FDC Servers - map downloads
31.13.71.1      |         | Facebook Ireland??   
94.100.180.236  | AS47764 | Mail.ru - Startup / Shutdown events are hardcoded to ping it

 etc.
 
 Known options to disable as of v9.4.1 (190910) 
 Settings:
  - Autodownload: Off (after initial download)
  - Backup Bookmarks: Off
  - Recent track (optional.. it's useful)
  - Send Statistics: Off
  - Google Play Services: (off)
  - Enable Logging: (OFF)
  - Mobile Internet: Never Use
  - Speed Cameras: Never
  - Crash Report: OFF
  
 
 To be clear, it is not OK for other applications to do this either.  Telemetry in mobile applications is a cancer that needs to die.
 
 Traffic was observed with passive interception.
