


### Steam
Steam is the content delivery platform created by Valve.  Understandably, there are many moving parts to it which I dont' take issue with.

Things to note:
- Most services are in clear text, not SSL.  That includes the Steam store.  Purchases are sent over SSL however it's pretty moot considering everything else isn't.
- Steam runs constantly in the background, frequently calling home for everything from icons to crash reports
- It is not possible to completely disable the steamcloud (hosted on Azure)
- Content servers have no political boundries, thus clients may end up downloading from anywhere in the world despite regional setting
  -- Verizon likes to hijack preference to their network
  

### hosts
```
# The more annoying hosts
127.0.0.2	nullroute1 steamcloudtoronto.blob.core.windows.net steamcloudtoronto.blob steamcloudlrsuswest.blob.core.windows.net steamclouduseast.blob.core.windows.net
127.0.0.3 crash.steampowered.com

# client-download.steampowered.com
# cdn.akamai.cs.steampowered.com
# cdn.akamai.steamstatic.com
# cdn.level3.cs.steampowered.com
# store.akamai.steamstatic.com.edgesuite.net a1737.g1.akamai.net store.akamai.steamstatic.com
# cdn.edgecast.steamstatic.com wpc.1d245.xicdn.net cs283.wpc.xicdn.net 1d245-lb.wpc.xicdn.net lb.apr-1d245.edgecastdns.net us-lb.1d245.ecdns.net gpla1.wpc.v1cdn.net store.edgecast.steamstatic.com
# cloud-3.steamusercontent.com cloud-3.steamusercontent.com.edgesuite.net a1639.g1.akamai.net
# media.steampowered.com media4.steampowered.com
# steamcloud-us.storage.googleapis.com


208.64.200.7 valve1.cs.steampowered.com
208.64.200.8 valve2.cs.steampowered.com
208.64.200.9 valve3.cs.steampowered.com
103.10.125.132 valve5.cs.steampowered.com
103.10.125.134 valve6.cs.steampowered.com
103.10.124.14 valve32.cs.steampowered.com
173.245.218.194 valve39.cs.steampowered.com
173.245.218.195 valve40.cs.steampowered.com
173.245.218.196 valve41.cs.steampowered.com
205.196.6.132 valve62.cs.steampowered.com
205.196.6.130 valve63.cs.steampowered.com
208.64.203.26 valve65.cs.steampowered.com
205.196.6.131 valve66.cs.steampowered.com
208.64.202.252 valve69.cs.steampowered.com
199.229.227.158 valve89.cs.steampowered.com
162.254.198.12 valve164.cs.steampowered.com
162.254.198.76 valve165.cs.steampowered.com
103.10.125.136 valve166.cs.steampowered.com
185.25.183.10 valve167.cs.steampowered.com
205.185.194.10 valve168.cs.steampowered.com
185.25.183.11 valve169.cs.steampowered.com
50.242.151.22 valve170.cs.steampowered.com
50.242.151.26 valve171.cs.steampowered.com
173.245.194.50 valve172.cs.steampowered.com
207.35.48.42 valve176.cs.steampowered.com
207.35.48.46 valve177.cs.steampowered.com
207.35.48.34 valve178.cs.steampowered.com
207.35.48.38 valve179.cs.steampowered.com
81.171.115.13 valve184.cs.steampowered.com
212.72.47.42 valve191.cs.steampowered.com
212.3.238.162 valve194.cs.steampowered.com
4.28.130.22 valve195.cs.steampowered.com
209.197.6.230 valve208.cs.steampowered.com
212.162.43.38 valve210.cs.steampowered.com
212.162.18.102 valve212.cs.steampowered.com
62.140.24.122 valve213.cs.steampowered.com
213.242.108.38 valve228.cs.steampowered.com
4.28.130.42 valve230.cs.steampowered.com
4.28.20.42 valve231.cs.steampowered.com
212.73.205.178 valve236.cs.steampowered.com
146.66.154.10 valve264.cs.steampowered.com
173.245.216.194 valve265.cs.steampowered.com
173.245.216.195 valve266.cs.steampowered.com
81.171.68.194 valve268.cs.steampowered.com
81.171.68.195 valve269.cs.steampowered.com
205.185.220.132 valve271.cs.steampowered.com
209.197.20.103 valve272.cs.steampowered.com
209.197.6.232 valve275.cs.steampowered.com
182.79.231.6 valve278.cs.steampowered.com
182.79.231.14 valve279.cs.steampowered.com
182.79.231.2 valve280.cs.steampowered.com
182.79.231.10 valve281.cs.steampowered.com
182.79.231.18 valve282.cs.steampowered.com
87.245.212.210 valve283.cs.steampowered.com
87.245.212.211 valve284.cs.steampowered.com
162.254.192.10 valve300.cs.steampowered.com
162.254.192.11 valve301.cs.steampowered.com
162.254.192.12 valve302.cs.steampowered.com
162.254.192.13 valve303.cs.steampowered.com
162.254.192.14 valve304.cs.steampowered.com
162.254.192.15 valve305.cs.steampowered.com
162.254.192.16 valve306.cs.steampowered.com
162.254.192.17 valve307.cs.steampowered.com
162.254.192.18 valve308.cs.steampowered.com
162.254.192.19 valve309.cs.steampowered.com
162.254.192.20 valve310.cs.steampowered.com
162.254.192.21 valve311.cs.steampowered.com
162.254.196.10 valve400.cs.steampowered.com
162.254.196.11 valve401.cs.steampowered.com
162.254.196.12 valve402.cs.steampowered.com
162.254.196.13 valve403.cs.steampowered.com
162.254.196.14 valve404.cs.steampowered.com
162.254.196.15 valve405.cs.steampowered.com
162.254.196.16 valve406.cs.steampowered.com
162.254.196.17 valve407.cs.steampowered.com
162.254.196.18 valve408.cs.steampowered.com
162.254.196.19 valve409.cs.steampowered.com
162.254.196.20 valve410.cs.steampowered.com
162.254.196.21 valve411.cs.steampowered.com
162.254.196.22 valve412.cs.steampowered.com
162.254.196.23 valve413.cs.steampowered.com
162.254.196.24 valve414.cs.steampowered.com
162.254.196.25 valve415.cs.steampowered.com
162.254.196.26 valve416.cs.steampowered.com
162.254.196.27 valve417.cs.steampowered.com
162.254.197.10 valve500.cs.steampowered.com
162.254.197.11 valve501.cs.steampowered.com
162.254.197.12 valve502.cs.steampowered.com
162.254.197.13 valve503.cs.steampowered.com
162.254.197.14 valve504.cs.steampowered.com
162.254.197.15 valve505.cs.steampowered.com
162.254.197.16 valve506.cs.steampowered.com
162.254.197.17 valve507.cs.steampowered.com
162.254.197.18 valve508.cs.steampowered.com
162.254.197.19 valve509.cs.steampowered.com
162.254.197.20 valve510.cs.steampowered.com
162.254.197.21 valve511.cs.steampowered.com
162.254.197.22 valve512.cs.steampowered.com
162.254.197.23 valve513.cs.steampowered.com
162.254.197.24 valve514.cs.steampowered.com
162.254.197.25 valve515.cs.steampowered.com
162.254.197.26 valve516.cs.steampowered.com
162.254.197.27 valve517.cs.steampowered.com
162.254.197.28 valve518.cs.steampowered.com
162.254.197.29 valve519.cs.steampowered.com
162.254.197.30 valve520.cs.steampowered.com
162.254.197.31 valve521.cs.steampowered.com
162.254.193.10 valve600.cs.steampowered.com
162.254.193.11 valve601.cs.steampowered.com
162.254.193.12 valve602.cs.steampowered.com
162.254.193.13 valve603.cs.steampowered.com
162.254.193.14 valve604.cs.steampowered.com
162.254.193.15 valve605.cs.steampowered.com
162.254.193.16 valve606.cs.steampowered.com
162.254.193.17 valve607.cs.steampowered.com
162.254.193.18 valve608.cs.steampowered.com
162.254.193.19 valve609.cs.steampowered.com
162.254.195.10 valve700.cs.steampowered.com
162.254.195.11 valve701.cs.steampowered.com
162.254.195.12 valve702.cs.steampowered.com
162.254.195.13 valve703.cs.steampowered.com
162.254.195.14 valve704.cs.steampowered.com
162.254.195.15 valve705.cs.steampowered.com
162.254.195.16 valve706.cs.steampowered.com
162.254.195.17 valve707.cs.steampowered.com
162.254.195.18 valve708.cs.steampowered.com
162.254.195.19 valve709.cs.steampowered.com
162.254.195.20 valve710.cs.steampowered.com
162.254.195.21 valve711.cs.steampowered.com
162.254.195.22 valve712.cs.steampowered.com
162.254.195.23 valve713.cs.steampowered.com
162.254.199.130 valve800.cs.steampowered.com
162.254.199.131 valve801.cs.steampowered.com
162.254.199.132 valve802.cs.steampowered.com
162.254.199.133 valve803.cs.steampowered.com
162.254.199.134 valve804.cs.steampowered.com
162.254.199.135 valve805.cs.steampowered.com
162.254.199.136 valve806.cs.steampowered.com
162.254.199.137 valve807.cs.steampowered.com
162.254.199.138 valve808.cs.steampowered.com
162.254.199.139 valve809.cs.steampowered.com
162.254.198.77 valve900.cs.steampowered.com
162.254.198.13 valve901.cs.steampowered.com
162.254.198.78 valve902.cs.steampowered.com
162.254.198.14 valve903.cs.steampowered.com
162.254.198.81 valve904.cs.steampowered.com
162.254.198.17 valve905.cs.steampowered.com
162.254.198.82 valve906.cs.steampowered.com
162.254.198.18 valve907.cs.steampowered.com
162.254.198.83 valve908.cs.steampowered.com
162.254.198.19 valve909.cs.steampowered.com
155.133.252.10 valve950.cs.steampowered.com
155.133.252.11 valve951.cs.steampowered.com
155.133.252.12 valve952.cs.steampowered.com
155.133.252.13 valve953.cs.steampowered.com
155.133.252.14 valve954.cs.steampowered.com
155.133.252.15 valve955.cs.steampowered.com
155.133.252.16 valve956.cs.steampowered.com
155.133.252.17 valve957.cs.steampowered.com
155.133.252.18 valve958.cs.steampowered.com
155.133.252.19 valve959.cs.steampowered.com
103.10.124.15 valve1000.cs.steampowered.com
162.254.193.24 valve614.steampipe.steamcontent.com
207.35.48.42 valve176.steampipe.steamcontent.com
207.35.48.46 valve177.steampipe.steamcontent.com
207.35.48.34 valve178.steampipe.steamcontent.com
207.35.48.38 valve179.steampipe.steamcontent.com
162.254.193.11 valve601.steampipe.steamcontent.com
162.254.193.14 valve604.steampipe.steamcontent.com
162.254.193.36 valve605.steampipe.steamcontent.com
162.254.193.37 valve606.steampipe.steamcontent.com
162.254.193.39 valve608.steampipe.steamcontent.com
162.254.193.40 valve609.steampipe.steamcontent.com
162.254.193.20 valve610.steampipe.steamcontent.com
162.254.193.21 valve611.steampipe.steamcontent.com
162.254.193.22 valve612.steampipe.steamcontent.com
162.254.193.23 valve613.steampipe.steamcontent.com
162.254.193.48 valve615.steampipe.steamcontent.com
162.254.193.49 valve616.steampipe.steamcontent.com
162.254.193.50 valve617.steampipe.steamcontent.com
162.254.193.51 valve618.steampipe.steamcontent.com
162.254.193.52 valve619.steampipe.steamcontent.com
208.64.201.169	cm0.steampowered.com
162.254.193.47 CM01-LON.cm.steampowered.com
CM01-ORD.cm.steampowered.com
CM01-LAX.cm.steampowered.com
CM01-STO.cm.steampowered.com
CM01-IAD.cm.steampowered.com
CM02-LON.cm.steampowered.com
CM02-ORD.cm.steampowered.com
CM02-LAX.cm.steampowered.com
CM02-STO.cm.steampowered.com
CM02-IAD.cm.steampowered.com
CM03-LON.cm.steampowered.com
CM03-ORD.cm.steampowered.com
CM03-LAX.cm.steampowered.com
CM03-STO.cm.steampowered.com
CM03-IAD.cm.steampowered.com
CM04-LON.cm.steampowered.com
CM04-ORD.cm.steampowered.com
CM04-LAX.cm.steampowered.com
CM04-STO.cm.steampowered.com
CM04-IAD.cm.steampowered.com
CM05-IAD.cm.steampowered.com
CM06-IAD.cm.steampowered.com 
```
