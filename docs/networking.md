**Table of Contents**
<!-- MarkdownTOC -->

- [Networking](#networking)
	- [Slides](#slides)
	- [NetDevOps Culture](#netdevops-culture)
	- [DNS](#dns)
	- [Next Generation Firewalls \(NGFW\)](#next-generation-firewalls-ngfw)
	- [Switches](#switches)
		- [Virtual LAN](#virtual-lan)
	- [Network virtualization. Software Defined Networking \(SDN\)](#network-virtualization-software-defined-networking-sdn)
		- [OpenDaylight](#opendaylight)
	- [IPv4](#ipv4)
	- [IPv6](#ipv6)
	- [Network Forensics](#network-forensics)
	- [Network Performance](#network-performance)
	- [CDN Content delivery network](#cdn-content-delivery-network)
	- [VoIP](#voip)
	- [MPLS Multi Protocol Label Switching \(IP VPN\)](#mpls-multi-protocol-label-switching-ip-vpn)
	- [BGP Border Gateway Protocol](#bgp-border-gateway-protocol)
	- [Mobile Core Network](#mobile-core-network)
	- [IMS IP Multimedia Subsystem](#ims-ip-multimedia-subsystem)
	- [IPTV Internet Protocol Television](#iptv-internet-protocol-television)
	- [WiFi security](#wifi-security)
	- [WiFi Products](#wifi-products)
	- [WebPerf and Resilient Networking: Planning for Failure](#webperf-and-resilient-networking-planning-for-failure)

<!-- /MarkdownTOC -->

![michael jordan](images/air_jordan.gif)

[![telcos vs web giants](images/telcos_vs_web_giants_spain.png)](http://www.zdnet.com/article/telcos-vs-the-web-giants-is-the-playing-field-a-fair-one-and-does-it-matter/)

[![top_10_telecom_providers](images/top_10_telecom_providers.jpg)](http://www.infonetics.com/pr/2013/1Q13-Service-Provider-Database-Highlights.asp)

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">New NYC buses are getting Wi-Fi and USB charging ports <a href="https://t.co/eGYCfy9irR">https://t.co/eGYCfy9irR</a> <a href="https://t.co/TQOAuWziyT">pic.twitter.com/TQOAuWziyT</a></p>&mdash; Mashable Tech (@mashabletech) <a href="https://twitter.com/mashabletech/status/707857779600584704">marzo 10, 2016</a></blockquote><script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">Jump start <a href="https://twitter.com/hashtag/mobile?src=hash">#mobile</a> in your <a href="https://twitter.com/hashtag/enterprise?src=hash">#enterprise</a> <a href="https://t.co/S0ndPhWGa6">https://t.co/S0ndPhWGa6</a> (via <a href="https://twitter.com/cmswire">@CMSWire</a>)</p>&mdash; Red Hat EMEA (@RedHatEMEA) <a href="https://twitter.com/RedHatEMEA/status/708692854495956992">12 de marzo de 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/4YgGuK9cuSU?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/_EBkBNQ00c0?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">Average internet speed, 2015 (megabytes per second)<br><br>Korea: 20.3<br>Sweden: 17<br>Norway: 16.4<br>Japan: 15<br>UK: 13<br>US: 12 <a href="https://t.co/kc9pWmrGJC">pic.twitter.com/kc9pWmrGJC</a></p>&mdash; The Int&#39;l Spectator (@intlspectator) <a href="https://twitter.com/intlspectator/status/711960597886164994">21 de marzo de 2016</a></blockquote><script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/iMduQ96N1F8?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/rA0NhPJOFyw?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

<center>

|[![gsma_video](images/gsma_video.jpg)](https://www.youtube.com/user/GSMAOnline)|[![telefonicaid](images/telefonicaid.jpg)](https://www.youtube.com/user/telefonicaid)|[![ericsson](images/ericsson.jpg)](https://www.youtube.com/c/ericsson)|[![telefonica_video_a_click_tic](images/telefonica_video_a_click_tic.jpg)](https://www.youtube.com/user/TelefonicaGGClientes)|
|:---:|:---:|:---:|:---:|

|[![opendaylight_video](images/opendaylight_video.jpg)](https://www.youtube.com/user/opendaylightproject)|[![opnfv_video](images/opnfv_video.jpg)](https://www.youtube.com/channel/UC3EjXLJbub0tPFpnI3vEmYg)|[![onf_video](images/onf_video.jpg)](https://www.youtube.com/user/OpenNetworkingFndn)|[![cisco_video](images/cisco_video.jpg)](https://www.youtube.com/user/Cisco)|[![huawei_enterprise_video](images/huawei_enterprise_video.jpg)](https://www.youtube.com/user/HuaweiEnterprise)|
|:---:|:---:|:---:|:---:|:---:|

|[![OPNFV_slides](images/OPNFV_slides.jpg)](http://www.slideshare.net/OPNFV)|[![opennetsummit_slides](images/opennetsummit_slides.jpg)](http://www.slideshare.net/opennetsummit)|![empty_youtube_channel](images/empty_youtube_channel.jpg)|![empty_youtube_channel](images/empty_youtube_channel.jpg)|[![wifisafe_video](images/wifisafe_video.jpg)](https://www.youtube.com/user/Wifisafe)|
|:---:|:---:|:---:|:---:|:---:|

|[![david_bombal_video](images/david_bombal_video.jpg)](https://www.youtube.com/user/ConfigTerm)|[![nick_feamster_video](images/nick_feamster_video.jpg)](https://www.youtube.com/user/nfeamster)|[![ivan_pepelvnjak_video](images/ivan_pepelvnjak_video.jpg)](https://www.youtube.com/user/IvanPx)|[![assaf_muller_video](images/assaf_muller_video.jpg)](assafmuller)|[![vmware_nsx_video](images/vmware_nsx_video.jpg)](https://www.youtube.com/user/vmwarensx)|
|:---:|:---:|:---:|:---:|:---:|

</center>

# Networking
## Slides
- [slideshare.net/Niasta](http://www.slideshare.net/Niasta) SDN, F5, Palo Alto, Juniper SRX, Wireless Security, VPN, Application Aware Networking, etc.

## NetDevOps Culture
- [blog.datapath.io: 10 Network Automation Principles for DevOps 🌟🌟🌟](http://blog.datapath.io/10-network-automation-principles-for-devops)
- [blog.datapath.io: What is NetDevOps?](http://blog.datapath.io/what-is-netdevops)
- [blog.datapath.io: What is Infrastructure as Code?](http://blog.datapath.io/what-is-infrastructure-as-code)

## DNS
- [DNS: What Can Go Wrong and How You Can Fix It | @DevOpsSummit #APM #Agile #DevOps](http://java.sys-con.com/node/3884842) DNS enables users of all skill sets and technical knowledge levels to use this incredibly advanced resource on a daily basis
- [DZone: How to Configure Your DNS With Cloud 66 for High Availability](https://dzone.com/articles/how-to-configure-your-dns-with-cloud-66-for-high-a) If you're using Cloud 66, here's a quick and easy tutorial to show you how to set your site up for high availability.
- [How To Flush Linux/UNIX DNS Cache](http://www.cyberciti.biz/faq/rhel-debian-ubuntu-flush-clear-dns-cache/)
- [unixmen.com: How To Setup DNS Server In Ubuntu 15.10](http://www.unixmen.com/how-to-setup-dns-server-in-ubuntu-15-10/)
- [linux.com: Dig Into DNS: Part 1](https://www.linux.com/learn/dig-dns-part-1)
- [blog.datapath.io: What is Domain Name System (DNS)?](http://blog.datapath.io/what-is-domain-name-system-dns)
- [blog.datapath.io: How we use Anycast for DNS Failover](http://blog.datapath.io/dns-failover-how-we-use-anycast-for-dns-failover)

[![dzone_refcard_practical_dns](images/dzone_refcard_practical_dns.png)](https://dzone.com/refcardz/dns)

## Next Generation Firewalls (NGFW)
- [Next Generation Firewalls (NGFW)](NGFW.md)

## Switches
- [reddit.com/r/networking](https://www.reddit.com/r/networking/)
- [SWITCH Security Report](http://securityblog.switch.ch/)
- [Layer 3 versus Layer 2 Switch for VLANs](https://documentation.meraki.com/MS/Layer_3_Switching/Layer_3_versus_Layer_2_Switch_for_VLANs)
- [Power over Ethernet or PoE](https://en.wikipedia.org/wiki/Power_over_Ethernet)
- [juniper switches](http://www.juniper.net/us/en/products-services/switching/)
- [Netgear switches](http://www.netgear.com/home/products/networking/switches/)
- [D-Link](http://www.dlink.com/uk/en/business-solutions/poe/switches)
- [Cisco Meraki](https://documentation.meraki.com/MS)
- [Cisco Small Business Switches](http://www.newegg.com/Switches/BrandSubCat/ID-12450-30)
- [Extreme](http://www.extremenetworks.com/products/switching-routing)
- [Linksys](http://www.linksys.com/us/c/business-network-switches/)
- [Dell](http://www.dell.com/us/business/p/switch-powerconnect)
- [HP Small and Midsize Business](http://www8.hp.com/us/en/networking/smb-networking-switches.html)
- [youtube: Dell Networking Z9100-ON 100GbE Fabric Switch](https://www.youtube.com/watch?v=GiGqRy5zgCM&feature=youtu.be)
- [The Top 10 Best Selling Switches By Brand](http://www.crn.com/slide-shows/networking/300072355/the-top-10-best-selling-switches-by-brand.htm)
- [Top 5 Small Business Switches](http://www.learncomputer.com/top-5-small-business-switches/)
- [community.spiceworks.com: Best 48 port small business switch?](https://community.spiceworks.com/topic/751984-best-48-port-small-business-switch)

<div class="container">
<iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/GiGqRy5zgCM?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">I FOUND IT. I FOUND THE INTERNET SWITCH. <a href="https://t.co/7xdOxhimI7">pic.twitter.com/7xdOxhimI7</a></p>&mdash; Whitney Champion (@shortxstack) <a href="https://twitter.com/shortxstack/status/707637919809404928">9 de marzo de 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/ddgQwtt8QCc?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br>

### Virtual LAN
- [Virtual LAN](VLAN.md)

## Network virtualization. Software Defined Networking (SDN)
- [opnfv.org FOSS Network Functions Virtualization](https://www.opnfv.org)
- [opennetworking.org](https://www.opennetworking.org/)
- [SDxCentral.com: Trusted News and Resources for SDx, SDN, NFV](https://www.sdxcentral.com/)
- [sdxcentral.com: What is NFV – Network Functions Virtualization?](https://www.sdxcentral.com/resources/nfv/whats-network-functions-virtualization-nfv/)
	- [Software-defined networking (SDN)](https://www.sdxcentral.com/flow/sdn-software-defined-networking/)
- [SDxCentral’s Top 10 News Stories of 2015](https://www.sdxcentral.com/articles/news/sdxcentrals-top-10-news-stories-of-2015/2016/01/)
- [sdxcentral.com: The Top NFV & Telecom Influencers in 2015](https://www.sdxcentral.com/articles/news/top-nfv-influencers-2015/)
- [aunclicdelastic.com: SDN, NFV y los fundamentos de las redes del futuro](http://www.aunclicdelastic.com/sdn-nfv-y-los-fundamentos-de-las-redes-del-futuro/)
- [Open Source MANO](http://osm.etsi.org) Open Source Mano is an ETSI-hosted project to develop an Open Source NFV Management and Orchestration (MANO) software stack aligned with ETSI NFV.
	- [Telefónica se une a otras 22 operadoras y proveedores de equipos para crear una comunidad global de Open Source Mano (OSM)](https://www.telefonica.com/es/web/sala-de-prensa/-/telefonica-se-une-a-otras-22-operadoras-y-proveedores-de-equipos-para-crear-una-comunidad-global-de-open-source-mano-osm-)
- [2016 Survey Shows More and Diverse SDN Use Cases Being Deployed by Open SDN Power Users](https://www.opendaylight.org/news/blogs/2016/02/2016-survey-shows-more-and-diverse-sdn-use-cases-being-deployed-open-sdn-power)
- [3 Trending Networking Skills Employers Look for in Open Source Pros 🌟🌟](https://www.linux.com/news/3-trending-networking-skills-employers-look-open-source-pros)
- [Single vendors don't offer a complete software-defined environment](http://searchnetworking.techtarget.com/news/450300354/Single-vendors-dont-offer-a-complete-software-defined-environment)
- [The telecoms industry and NFV – How the cloud is virtualising](http://www.vanillaplus.com/2016/08/04/20138-the-telecoms-industry-and-nfv-how-the-cloud-is-virtualising/)
- [Automation is Paramount in Cloud/NFV (Infographic) 🌟🌟🌟](http://blog.dialogic.com/blog/automation-is-paramount-in-cloud/nfv-infographic)
- [sdxcentral.com: What Are Microservices in NFV? Definition 🌟](https://www.sdxcentral.com/nfv/definitions/microservices-in-nfv-definition) 
- [opensource.com: Managing networks in a software-defined future](https://opensource.com/business/16/7/managing-networks-software-defined-future)
- [blog.datapath.io: What is Software Defined Networking (SDN)?](http://blog.datapath.io/what-is-software-defined-networking-sdn)
- [blog.datapath.io: What is Network Function Virtualization (NFV)?](http://blog.datapath.io/network-function-virtualization-nfv)

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">Great interview w/ <a href="https://twitter.com/darrelljs">@darrelljs</a> &amp; <a href="https://twitter.com/intel">@intel</a> John Healy discussing &quot;The Future of NFV&quot; <a href="https://twitter.com/TIA_Now">@TIA_Now</a> <a href="https://twitter.com/hashtag/MWC16?src=hash">#MWC16</a> <a href="https://twitter.com/OpenTelco">@OpenTelco</a> <a href="https://twitter.com/hashtag/redhat?src=hash">#redhat</a> <a href="https://t.co/NzB8p1Qur1">https://t.co/NzB8p1Qur1</a></p>&mdash; Annie Potvin (@anniep0206) <a href="https://twitter.com/anniep0206/status/702396797063454722">febrero 24, 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr"><a href="https://twitter.com/hashtag/NFV?src=hash">#NFV</a> and <a href="https://twitter.com/hashtag/SDN?src=hash">#SDN</a> represent a huge step for the industry and a big change in how networks are designed and built <a href="https://t.co/m1MY1eVUCp">https://t.co/m1MY1eVUCp</a></p>&mdash; SDNspace (@SDNspace) <a href="https://twitter.com/SDNspace/status/773068130474160128">6 de septiembre de 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/f9_Zb2npybA?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

[![att_nw_virtualization](images/att_nw_virtualization.jpg)](http://www.rcrwireless.com/20160712/fundamentals/domain-2-0-tag31-tag99)

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/HFQdbOY8Ams?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

<div class="container">
<iframe src="//www.slideshare.net/slideshow/embed_code/key/AErpa2kNvJd73E" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen class="video"> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/Ericsson_ES/el-sector-de-las-tic-en-espaa-santander-2013-ericsson" title="El sector de las tic en españa santander 2013 - ericsson" target="_blank">El sector de las tic en españa santander 2013 - ericsson</a> </strong> from <strong><a href="//www.slideshare.net/Ericsson_ES" target="_blank">Ericsson España</a></strong> </div>
</div>
<br/>

<div class="container">
<iframe src="//www.slideshare.net/slideshow/embed_code/key/2Me02xGBOaDGWQ" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen class="video"> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/basimaly1/introduction-to-sdn-and-nfv" title="Introduction to SDN and NFV" target="_blank">Introduction to SDN and NFV</a> </strong> from <strong><a href="//www.slideshare.net/basimaly1" target="_blank">Basim Aly (JNCIP-SP, JNCIP-ENT)</a></strong> </div>
</div>
<br/>

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/-c5P2CvBTRg?list=PLk1Rzj8ppcXm7jv58Hrr6jv1t8A-OHVfA" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

<div class="container">
<iframe src="//www.slideshare.net/slideshow/embed_code/key/w0I4y28c9OTwZy" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen class="video"> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/Niasta/sdn-software-defined-networking-and-nfv-network-function-virtualization" title="SDN- Software Defined Networking and NFV- Network Function Virtualization" target="_blank">SDN- Software Defined Networking and NFV- Network Function Virtualization</a> </strong> from <strong><a target="_blank" href="//www.slideshare.net/Niasta">Niasta</a></strong> </div>
</div>
<br/>

### OpenDaylight
-  With the rise of cloud computing and the expansion of data centers, software-defined solutions, like this Linux-based platform, are gaining greater traction in the tech industry. OpenDaylight works to help drive network success, reduce business costs and provide employees with greater flexibility.
- [opendaylight.org](https://www.opendaylight.org)

<div class="container">
<iframe src="//www.slideshare.net/slideshow/embed_code/key/iAm4HSH0q1R1K9" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen class="video"> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/esumit/opendaylight-sdn-controller" title="Opendaylight SDN Controller" target="_blank">Opendaylight SDN Controller</a> </strong> from <strong><a href="//www.slideshare.net/esumit" target="_blank">Sumit Arora</a></strong> </div>
</div>
<br/>

<div class="container">
<iframe src="//www.slideshare.net/slideshow/embed_code/key/elWbuAzg3IbcH5" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen class="video"> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/sdnhub/opendaylight-app-development-tutorial" title="OpenDaylight app development tutorial" target="_blank">OpenDaylight app development tutorial</a> </strong> from <strong><a href="//www.slideshare.net/sdnhub" target="_blank">SDN Hub</a></strong> </div>
</div>
<br/>

## IPv4
- [wikipedia: IPv4](https://en.wikipedia.org/wiki/IPv4)

<div class="container">
<iframe src="//www.slideshare.net/slideshow/embed_code/key/efHHF5aHeCPyv" width="668" height="714" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen class="video"> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/UmerQureshi9/simple-ipv4subnetting" title="Simple IPv4_Subnetting" target="_blank">Simple IPv4_Subnetting</a> </strong> from <strong><a href="//www.slideshare.net/UmerQureshi9" target="_blank">Umer Qureshi</a></strong> </div>
</div>
<br/>

<div class="container">
<iframe src="//www.slideshare.net/slideshow/embed_code/key/EnfPCPLoYI8A9Q" width="668" height="714" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen class="video"> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/swapnilkapate/i-pv4-subnetting-16465968" title="I pv4 subnetting" target="_blank">I pv4 subnetting</a> </strong> from <strong><a href="//www.slideshare.net/swapnilkapate" target="_blank">Swapnil Kapate</a></strong> </div>
</div>
<br/>

<div class="container">
<iframe src="//www.slideshare.net/slideshow/embed_code/key/NTUP0U3kq421kQ" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen class="video"> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/nilmenon/ccna-1-routing-and-switching-v50-chapter-9" title="CCNA 1 Routing and Switching v5.0 Chapter 9" target="_blank">CCNA 1 Routing and Switching v5.0 Chapter 9</a> </strong> from <strong><a href="//www.slideshare.net/nilmenon" target="_blank">Nil Menon</a></strong> </div>
</div>
<br/>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="es" dir="ltr">Telefónica se une a 22 operadoras y proveedores de equipos para crear una comunidad global Open Source Mano <a href="https://twitter.com/hashtag/MWC16?src=hash">#MWC16</a> <a href="https://t.co/gCRmbpHduW">https://t.co/gCRmbpHduW</a></p>&mdash; Telefónica (@Telefonica) <a href="https://twitter.com/Telefonica/status/701724993441415168">febrero 22, 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">The future of Wi-Fi Is 10,000 times more energy efficient <a href="https://t.co/uaAsPJ2J0R">https://t.co/uaAsPJ2J0R</a></p>&mdash; WIRED (@WIRED) <a href="https://twitter.com/WIRED/status/706244154184089600">5 de marzo de 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="es" dir="ltr">Fibra óptica, el mejor vehículo para viajar hacia la nube ➡ <a href="https://t.co/zUq9TK7Smd">https://t.co/zUq9TK7Smd</a> <a href="https://twitter.com/hashtag/Conectividad?src=hash">#Conectividad</a> <a href="https://twitter.com/hashtag/Pymes?src=hash">#Pymes</a></p>&mdash; Movistar pymes (@Movistar_pymes) <a href="https://twitter.com/Movistar_pymes/status/706232959653830662">5 de marzo de 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

## IPv6
- [wikipedia: IPv6](https://en.wikipedia.org/wiki/IPv6)
- [arstechnica.com: IPv6 celebrates its 20th birthday by reaching 10 percent deployment](http://arstechnica.com/business/2016/01/ipv6-celebrates-its-20th-birthday-by-reaching-10-percent-deployment/)
- [opensource.com: 8 reasons to make the switch to IPv6](https://opensource.com/business/16/1/scale14x-interview-owen-delong-akamai-technologies)

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">8 reasons to make the switch to IPv6: <a href="https://t.co/DBdU0Ap6Xv">https://t.co/DBdU0Ap6Xv</a></p>&mdash; Open Source Way (@opensourceway) <a href="https://twitter.com/opensourceway/status/706178465226104833">5 de marzo de 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<div class="container">
<iframe src="//www.slideshare.net/slideshow/embed_code/key/jNw65ZLpdYJz4Y" width="595" height="485" frameborder="0" marginwidth="0" marginheight="0" scrolling="no" style="border:1px solid #CCC; border-width:1px; margin-bottom:5px; max-width: 100%;" allowfullscreen class="video"> </iframe> <div style="margin-bottom:5px"> <strong> <a href="//www.slideshare.net/shaileshpachori/master-all-home" title="Ipv4 vs Ipv6 comparison" target="_blank">Ipv4 vs Ipv6 comparison</a> </strong> from <strong><a href="//www.slideshare.net/shaileshpachori" target="_blank">Shailesh Pachori</a></strong> </div>
</div>
<br>

## Network Forensics
- [Network Forensics](nw_forensics.md)

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/CXVINBruzhY?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

## Network Performance
- [Network Performance](nw_performance.md)

## CDN Content delivery network
- [CDN Content delivery network](cdn.md)

## VoIP
- [VoIP](voip.md)

## MPLS Multi Protocol Label Switching (IP VPN)
- [tech-faq.com: MPLS](http://www.tech-faq.com/mpls.html)
- [Why Cloud is making MPLS obsolete - and how Service Providers can adapt](https://www.linkedin.com/pulse/20140915110843-538739-why-cloud-is-making-mpls-obsolete-and-how-service-providers-can-adapt)
- [Software-defined wide-area network, Is this the end of MPLS VPNs?](https://www.linkedin.com/pulse/software-defined-wide-area-network-end-mpls-vpns-greg-de-chasteauneuf)
- [MPLS vs. Metro-Ethernet](https://www.linkedin.com/pulse/mpls-vs-metro-ethernet-dave-calhoun)

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/E5Ud1m9h0yc?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/AtmmbsQTSa8?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

## BGP Border Gateway Protocol 
- [Using Border Gateway Protocol for Latency Optimization](http://blog.datapath.io/using-border-gateway-protocol-for-latency-optimization)
- [How BGP Best Path Selection Works](http://blog.datapath.io/how-bgp-best-path-selection-works)
- [How we use iBGP at Datapath.io](http://blog.datapath.io/how-we-use-ibgp-at-datapath.io)

## Mobile Core Network
- [Mobile Core Network](mobilecore.md)

## IMS IP Multimedia Subsystem
- [IMS IP Multimedia Subsystem](ims.md)

## IPTV Internet Protocol Television
- [IPTV](iptv.md)

## WiFi security
- [Analyzing the 1000 Most Common Wi-Fi Network Names](https://ghostpath.com/blog/ssid-analyzing-the-1000-most-common-wi-fi-network-names/)
	- [Recommend Length for Wi-FI PSK?](http://security.stackexchange.com/questions/15653/recommend-length-for-wi-fi-psk)
	- [Is a WPA/WPA2 Wi-Fi network secure?](https://www.acrylicwifi.com/en/blog/is-a-wpawpa2-wi-fi-network-secure/)
	- [wikipedia: Wi-Fi Protected Access](https://en.wikipedia.org/wiki/Wi-Fi_Protected_Access)
- [Ubiquiti Networks](https://www.ubnt.com)
- [Aruba Networks](http://www.arubanetworks.com)
- [HP Acquires Aruba Networks to Create an Industry Leader in Enterprise Mobility](http://www8.hp.com/hpnext/posts/hp-announcement-march-2015)
- [zdnet: DD-WRT Linux firmware comes to Linksys routers](http://www.zdnet.com/article/dd-wrt-linux-firmware-comes-to-linksys-routers/)

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/6pYZ2N9y2fQ?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

## WiFi Products
- [twitter.com/wifisafespain](https://twitter.com/wifisafespain)
- [The Best Wi-Fi Routers: No More Dead Zones](http://www.wsj.com/articles/these-routers-fix-wi-fi-dead-zones-but-theyll-cost-you-1469038426)
- [DD-WRT](https://en.wikipedia.org/wiki/DD-WRT)

[![wifisafe](images/wifisafe-marca.jpg)](https://www.wifisafe.com/)

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">Cool. How Wi-Fi waves propagate in a building. <a href="https://twitter.com/hashtag/networking?src=hash">#networking</a> <a href="https://twitter.com/hashtag/WiFi?src=hash">#WiFi</a> <a href="https://t.co/VvB8sQwYE7">pic.twitter.com/VvB8sQwYE7</a></p>&mdash; nixCraft (@nixcraft) <a href="https://twitter.com/nixcraft/status/736534890137550848">28 de mayo de 2016</a></blockquote><script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/xmabFJUKMdg?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="ht" dir="ltr">Lmao. <a href="https://t.co/wKsRGwma9K">pic.twitter.com/wKsRGwma9K</a></p>&mdash; nixCraft (@nixcraft) <a href="https://twitter.com/nixcraft/status/759077177140752385">29 de julio de 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

## WebPerf and Resilient Networking: Planning for Failure
- [WebPerf & Resilient Networking: Planning for Failure. Service Worker tool, wireless and mobile network optimization](https://www.igvita.com/2015/01/26/resilient-networking/)
	- [HTML5: Introduction to Service Worker](http://www.html5rocks.com/en/tutorials/service-worker/introduction/)
- [10 emuladores WAN para que pruebes distintas condiciones de red](http://www.hackplayers.com/2015/10/10-emuladores-wan-para-que-pruebes.html)
- [NEWfly, Redes Cisco y Packet Tracker: Network, ejercicios Packet Tracer y simulación de vuelo](https://newfly.wordpress.com/)

[![lifehacker_vpn_comparison](images/lifehacker_vpn_comparison.png)](http://lifehacker.com/this-massive-vpn-comparison-spreadsheet-helps-you-choos-1764427219)

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">Internet cables under the sea that connects continents together. This is how they put the cables. <a href="https://t.co/K8WbrgoOEW">pic.twitter.com/K8WbrgoOEW</a></p>&mdash; nixCraft (@nixcraft) <a href="https://twitter.com/nixcraft/status/705260332982231041">3 de marzo de 2016</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/IlAJJI-qG2k?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">Latest submarine internet/telephone cable maps 2016 edition. Large version [3737x1818] <a href="https://t.co/32MZ0c4U6g">https://t.co/32MZ0c4U6g</a> <a href="https://t.co/sNFBRBJsKg">pic.twitter.com/sNFBRBJsKg</a></p>&mdash; nixCraft (@nixcraft) <a href="https://twitter.com/nixcraft/status/711766471827791872">21 de marzo de 2016</a></blockquote><script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<blockquote class="twitter-tweet tw-align-center" data-lang="es"><p lang="en" dir="ltr">So cool. A GIF Illustrating The Rise Of The Internet i.e. Submarine Cables. <a href="https://twitter.com/hashtag/networking?src=hash">#networking</a> <a href="https://t.co/hPk97CIpXV">pic.twitter.com/hPk97CIpXV</a></p>&mdash; nixCraft # (@nixcraft) <a href="https://twitter.com/nixcraft/status/773388094624112640">7 de septiembre de 2016</a></blockquote><script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>

<p align="center">
<a href="http://www.buzzfeed.com/lukebailey/satisfying-cables">23 Photos That Will Make 
Anyone Who Works In IT Satisfied</a>
</p>
[![cabling](images/cabling.jpg)](http://www.buzzfeed.com/lukebailey/satisfying-cables)

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/c8AAQ1iH7FU?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/pwgmuEfrKCw?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>

<div class="container">
<iframe width="560" height="315" src="https://www.youtube.com/embed/jpLKU6-4T7Q?rel=0" frameborder="0" allowfullscreen class="video"></iframe>
</div>
<br/>


