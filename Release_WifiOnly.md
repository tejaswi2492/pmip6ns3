# Introduction #

PMIPv6 codes for NS-3 network simulator

New release: [ns-allinone-3.12.1-pmip6\_wifionly.tar.xz](http://code.google.com/p/pmip6ns3/downloads/detail?name=ns-allinone-3.12.1-pmip6_wifionly.tar.xz&can=2&q=)

# Details #

## Changes: ##
  * Supports UDP6 application.
  * Supports Wifi network only.
  * The list of ns3::TunnelNetDevice is managed by std::map instead of std::list
  * Bugfix: visualizer tooltip crash on ipv6-enabled node
  * Bugfix: NS now can use link-local address as a source address


## How to Install: ##

### By Download ###

  1. Download the release
    * By browser: click [here](http://code.google.com/p/pmip6ns3/downloads/detail?name=ns-allinone-3.12.1-pmip6_wifionly.tar.xz&can=2&q=).
    * By wget command: `wget http://pmip6ns3.googlecode.com/files/ns-allinone-3.12.1-pmip6_wifionly.tar.xz`
  1. Extract the file
    * `tar xvfJ ns-allinone-3.12.1-pmip6_wifionly.tar.xz`

### By Mercurial ###
  1. Clone repository to local folder:
    * `hg clone https://code.google.com/p/pmip6ns3.12#pmip6ns3.12-wifionly ns-allinone-3.12.1-pmip6`


## How to Excute the simulation: ##
  1. Change directory
    * `cd ns-allinone-3.12.1-pmip6`
    * `cd ns-3.12.1`
  1. Configure
    * `./waf -d debug configure`
  1. Build
    * `./waf`
  1. Run
    * `./waf --run pmip6-wifi`