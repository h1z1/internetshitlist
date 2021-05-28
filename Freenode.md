


Freenode **should not be used for really anything**. 

Do not confuse Freenode with other networks nor IRC itself.  EFNet for example.


CLOAKS
------
Freenode "Cloaks", are not the same as spoofing on other networks. General operators and apaprently end users are able to reveal the IP behind any cloak. Freenode does not see a problem with this. 

More daming is the aparent policy of staff to kill split servers even though they may have users whom are connected without issue.   Reconnecting requires reauthenticating with NICKSERV before a cloak is reapplied.


STAFF
-----
Deny, deny, deny ... Staff are largely unhelpful, outright arrogant especially when it comes to security and operational issues.  See discussions with staff.


CHANNELS
--------
Unlike other networks, Freenode allows channel registration which leads to lovely cases where channels are squated or more hillariously, reserved by Freenode themselves.



USERS NAMES
------------
Unlike other networks, Freenode allows nick registration which leads to lovely cases where nicks are squated or more hillariously, reserved by Freenode themselves.


CODE/SERVERS
------------

Code cannot be vetted as it's closed to Freenode Inc.

Freenode is a commercial organization which maintains every server, as such no process be it code or security can be vetted.


INTERCEPTION
------------

Under the guise of spam control, Freenode added the ability for every message, public or private, to be intercepted and scanned for "malicious intent".  They claim this is not possible to reverse and used for general logging as it's based on hashing..  That not only makes no sense but further indicates how clueless this organization is wrt security or privacy.


SERVER LOCATIONS
----------------

It is not possible as an end user to list what servers are connected, nor where they are located.  This is especially concerning with hubs as they become central points of interception -legal or otherwise.


CERTIFICATE USE
---------------

Server SSL certifcates have several times changed with no notice nor warning to users.  They were not expired but regenerated entirely.



HOST NAMES
---------

irc.freenode.net is an alias for chat.freenode.net.

No where near the servers connected

-!- There are 97 users and 83728 invisible on 30 servers


| Host | Location | IP
| ---------------------- | ---------------- | ----------- | 
|karatkievich.freenode.net | [Montreal, CA] |	64.86.243.181 |
|hitchcock.freenode.net | [Sofia, BG, EU] | 	130.185.232.126 |
|livingstone.freenode.net | [New York City, NY, US] |107.182.226.199 |
|adams.freenode.net | [Budapest, HU, EU] |	94.125.182.252 |
|sinisalo.freenode.net | [SE, EU] |91.217.189.42 |
|weber.freenode.net | [US] |162.213.39.42 |
|niven.freenode.net | [London, UK, EU] |139.162.227.51 |
|tolkien.freenode.net | [Sanford, NC, US] |204.225.96.251 |
|barjavel.freenode.net | [Paris, FR, EU] |195.154.200.232 |
|wolfe.freenode.net | [Stockholm, SE, EU] |193.10.255.100 |
|leguin.freenode.net | [Umeå, SE, EU] |130.239.18.119 |
|orwell.freenode.net | [Amsterdam, NL, EU] |185.30.166.37 |
|kornbluth.freenode.net | [Frankfurt, Germany] |82.96.96.11 |
|zettel.freenode.net | [Tor] | Tor |


UPDATE:  Freenode drama has caused the network as a whole to split.  As such serveral "staff" of Freenode have annouced their "resignations".  Not sure how that is possible given they were never employed to begin with.

Examples:

https://gist.github.com/aaronmdjones/1a9a93ded5b7d162c3f58bdd66b8f491


Noteworthy disclosure:

> Before September 2020, the development effort was being spent on upstream
> Charybdis instead, since at least December 2019 (see [8] through [41] for
> details, inclusive), with edk (head of our development team) doing almost
> all of the work. The intention was that freenode would be migrating to
> Charydis when it was ready. That plan fell apart because of unrelated
> drama, and Charybdis was forked (again) at that point.
>   
> The work being done on Charybdis, and Solanum since, was in an effort to
> make the network easier to administer, and allow for the implementation
> of new IRCv3 features, such as message IDs (necessary for message
> editing and deletion) and BRB/RESUME support.
   
   
That is not IRC, it's a continuation of the bastard stepchild known as Slack and should never be accepted.  IRC is ephemeral by design.


Current Freenode server list includes 45.58.138.170 which as of this update does not resolve to anything but believed to be a test server known as tildes.freenode.net.  In production.

Server is hosted out of the UK by Chineese company known as Sharktech

```
route:      45.58.128.0/18
descr:      Sharktech Inc.
origin:     AS46844
mnt-by:     MAINT-AS46844
changed:    timt@sharktech.net 20170821  #23:49:34Z
source:     RADB

route:          45.58.128.0/18
descr:          Sharktech Inc.
origin:         AS46844
mnt-by:         MNT-SHARK-7
changed:        timt@sharktech.net  20150317
source:         ARIN
```

   Name Server: NS1.SHARKTECH.NET
   Name Server: NS2.SHARKTECH.NET


```
$ host sharktech.net
sharktech.net has address 170.178.191.84
sharktech.net mail is handled by 10 chi-pmg.sharktech.net.

$ whois 170.178.191.1
route:      170.178.191.0/24
descr:      CMI  (Customer Route)
origin:     AS46844
mnt-by:     MAINT-AS58453
changed:    qas_support@cmi.chinamobile.com 20180502
source:     RADB

route:      170.178.191.0/24
descr:      CMI IP Transit
origin:     AS46844
admin-c:    MAINT-CMI-INT-HK
tech-c:     MAINT-CMI-INT-HK
mnt-by:     MAINT-CMI-INT-HK
changed:    qas_support@cmi.chinamobile.com 20180503
source:     NTTCOM

route:          170.178.160.0/19
descr:          Sharktech Inc.
origin:         AS46844
mnt-by:         MNT-SHARK-7
changed:        timt@sharktech.net  20150317
source:         ARIN

mntner:         MAINT-CMI-INT-HK
descr:          China Mobile International Limited
country:        HK
admin-c:        CMIL1-AP
upd-to:         qas_support@cmi.chinamobile.com
auth:           # Filtered
mnt-by:         MAINT-CMI-INT-HK
referral-by:    APNIC-HM
last-modified:  2017-11-22T09:00:43Z
source:         APNIC
```

