---
title: Towards Environmental Sustainability with the IETF
type: blog
date: 2021-12-08
imageurl: /assets/preview_ict_for_sustainability.png
imagedsc: Part of the cover of the 2nd issue of the Branch magazine.
authors: Christoph Becker
---

<!-- Setting the stage for ICT -->
Information and communications technology (ICT) has played an important role in promoting the transition of society, technology, and economy from the industrial to the information era. Now, the transformation of society from an information to a sustainable (First time I've seen "s12y" (sustainability) and while I'm usually averse to new buzzwords I quite like the association with "i18n" (internationalization) and "a11y" (accessibility).) future (variously denoted as post-anthropocenic, -cthulucenic, or -capitalocenic epoch) is being imagined to use the same technology. Reason being is, that ICT is said to increase the energy efficiency of the economy in general, which currently wastes appr. 86% of the produced energy [[3]](#3). For the energy sector specifically, it would enable a distributed and decentralised energy networks, which would shorten power transmission routes, decrease energy waste, and reduce greenhouse gas (GHG) emissions.


<!-- Need to improve ICT -->
If the ICT sector is to play such a pivotal role in the energy transition, it will take on a significant burden to reduce it's own energy consumption and GHG emissions.
While it currently contributes 2.1-3.9% to the total GHG emission of our population (C. Freitag et al 2021), it is projected to dramatically increase within this decade: using 21% of global electricity by 2030 in the expected case, with an 8% or 51% share in the best and worst cases respectively [1]. The most significant trend along this projection, regardless of scenario, is that the energy consumption decreases in consumer devices and increases in networks and data centers. The transformative potential of 5G, on the energy sector specifically and the economy and society in general, puts the Internet infrastructure at the center of discussions about sustainable development and begs for in depth and cross-disciplinary deliberation.


<!-- Introducing SDOs -->
In this short article, I want to explore how standards-developing organisations (SDO) have so far attended to the climate emergency. While not all Internet governance practices unfold in standard-setting institutions, these bodies are focus points for coordination, and a place where many of the actors that produce the Internet, and exercise infrastructural power, meet. They pose as a space for self-regulated fora and bottom-up coordination (Sowell 2012 and ten Oever 2021). There are a number of relevant SDOs who's work on Internet governance and standardisation is done in cooperation with other SDOs and whos focus can evolve into different directions. To simplify this exploration, I will only focus on the principal SDOs engaged in the development of the Internet’s architecture, namely the Internet Engineering Task Force (IETF) and the World Wide Web Consortium (W3C).


<!-- TCP/IP protocol stack -->
Before uncovering the histories of climate thought in the chosen SDOs, let's sketch the essential parts of the Internet to gain an overview of where potential improvements can be made. The most universal, high-level, and persistent element of structure and organisation is the network architecture. The architecture defines how sets of protocols are organised, where protocols define how various modules interact. For the current Internet, the architecture design is the TCP/IP protocol stack (also referred to as the hourglass protocol stack). Although in theory each protocol belongs to one layer in the stack, in practice protocols were required that can 'overlay' between different layers. Thus, even though the image of a tidy stack of separate sets of protocols is outdated, I will list it here as it is what we currently have to work with. As a side note, notable research projects that study new architecture designs are SCION, RINA and NDN.

| Layer         | SDO          | Standards
| ------------- | ------------ | ---------------
| 4 Application | IETF         | HTTP, HTML, MIME, POP, IMAP, SMTP, DNS, SSH
|               | W3C          | HTTP, HTML, XML
|               | ITU-T        | JPEG
| 3 Transport   | IETF         | TCP, UDP, TLS, QUIC
| 2 Internet    | IETF         | IPv4, IPv6, ICMP, ECM, Seamoby
| 1 Network     | IEEE         | Ethernet, WiFi
|               | ITU-T        | ISDN, DSL
|               | 3GPP         | 2G/3G/4G/5G


<!-- ITU -->
All five standardisation bodies in the table have and are working towards a sustainable future. The International Telecommunication Union-Telecommunication Standardisation Sector (ITU-T) investigates within its Study Group 5 environmental effects of ICT and published guidelines for using ICT in an eco-friendly way. It is also responsible for studying design methodologies to reduce environmental effects. ITU-T L.1200 specifies the Direct Current interfaces while ITU-T L.1300 describes best practices to reduce negative impact of datacenters on climate.


<!-- 3GPP -->
The 3rd Generation Project Partnership (3GPP) was founded by the European Telecommunications Standards Institute (ETSI). In 2014, ETSI published standard ES-203-237 "Green Abstraction Layer" that specifies the Green Standard Interface (GSI) and the Energy Aware States (EASes) to establish uniform interactions between the energy-aware hardware and the control framework. The goal of this standard was to represent an abstraction of the energy-aware capabilities of networking devices to higher-layer protocols.


<!-- W3C -->
The World Wide Web Consortium (W3C) had a 'Climate action, environment, resource efficiency and raw materials Community Group' which existed for appr. one year until 2016. It was established under the 'Big Data Europe' project under the European Union's Horizon 2020 Programme. It mainly served the purpose to '[to identify the current as well the future Big Data challenges in the Climate domain](https://www.w3.org/community/bde-climate/2015/09/04/summary-of-1st-community-bde-sc5-workshop/)'. The outcomes would then be used to design and realise the ICT infrastructure needed to benefit from big data technologies, maximising the opportunities of the latest European RTD developments, including multilingual data harvesting, data analytics, and data visualisation. Although this community group was only short lived, continues and newer traces of climate thought can be found within W3C. Such as in 2019 when W3C's Technical Architecture Group released their ['Ethical Web Principles'](https://www.w3.org/2001/tag/doc/ethical-web-principles/#sustainable) which explicitly states: 'The web must be an environmentally sustainable platform'. These principles have been labelled as 'anticompetitive' within W3C and shows the competition of views within SDOs. A recently erupted debate around W3C efforts to standardise Decentralized Identifiers (DID), a prominent use case of the infamous non-fungible tokens (NFT). It started with the Mozilla Foundation's  [call to review](https://lists.w3.org/Archives/Public/public-new-work/2021Sep/0000.html) W3C's DID v1.0 in September 2021 as:

> Proof-of-work methods (e.g. blockchains) are harmful for sustainability (s12y). Also as noted by Google, the registry contains methods which rely upon proof-of-work which is wasteful. “Successful” proof-of-work systems waste a staggering amount of electricity world-wide (e.g. Bitcoin consumes more energy than most countries [...]) demonstrating that the more such methods are adopted, the more their energy requirements grow, without any discernible upper bound, which is grossly irresponsible given the global environmental crisis (recent IPCC report [...]).

To which the responds of W3C's DID working group members was:

> It seems like a witch hunt.

> This is a blatant political attack on cryptocurrencies and has no place in interoperability specifications for DID Methods.

None the less, it was agree to include a section on 'Environmental Considerations' in the [current draft](https://w3c.github.io/did-imp-guide/#environmental-considerations).


<!-- IETF -->
The Internet Engineering Task Force (IETF) is among the most open and transparent Internet SDOs.

A clear example of IETF's influence is given by its redesign of the IPv4 communication protocol into the improved version IPv6. The redesign does not only solve the problem of IPv4 address exhaustion, but also reduces energy waste and increases flexibility towards green networking (e.g., [[7]](#7), [[8]](#8), [[9]](#9), [[10]](#10)). In 2010, the IETF set up the Energy Management working group (EMAN, [[11]](#11)) to create a framework standard that enables monitoring, controlling, and managing the energy consumption of networking and network-attached devices while still providing sufficient performance to meet service level objectives with Five years later however, the EMAN working group was shut down and has never been reactivated despite remaining limitations (e.g., it does not address questions regarding electricity producers, and distributors) and the roll-out of new technologies (e.g., IoT and 5G). But other dimensions through which impacts on climate and ecology can be addressed are present in other working groups that are concerned with, e.g., smart energy, smart grid, and the Internet of Things.

The IETF is one of the main Internet governance bodies and it is therefore pressing to ask what its role ought to be, can be, and currently is with respect to climate change.
On the other hand, IETF Eman (Internet Engineering Task Force-Energy Management) studies several MIBs for energy management of network devices in ICT systems for international standardisation actively. These MIBs are based on SNMPs but all drafts by EMAN are caught in the proposal stage (e.g. RFC 7603 which hasn't considered security issues of SNMPs, as the reviewr writes "This necessarily extends to monitoring, and there is certainly a *lot* of information that may be gleaned by an attacker from monitoring power consumption,").


At present, the proposed energy-efficient methods are usually divided into two classes: one is on device-level, which provides the energy-efficient network devices and terminals; the other is on system-level, which organises the usage of devices and terminals energy-efficiently in a network-wide manner. The energy-efficient routing algorithm belongs to system-level energy saving scheme, which aims to find the most energy-efficient route for users and thus reduce energy consumption when transferring traffic along the route.




Now, the ICT sector is in a similar situations and various 'ICT for Sustainability' ([ICT4S](https://conf.researchr.org/series/ict4s)) and Green IT initiatives have cropped up over the years. Thus

And here, it is worthwhile to dwell on the what this space 'elsewhere' is. However, the observation that decreasing a processes resource intensity does not lead to a decrease in overall consumption, has already been described by Stanley Jevons in his 1865 work "The Coal Question". The so called "Jevons paradox" has since then always gone alongside the pursued to increasing efficiency and economic growth. Taking LEDs as an example, 'elsewhere' has come to be a very large space indeed. Their appr. 60% lower environmental impact than fluorescent luminaire [[12]](#12), and more so their impression of 'advanced technology', has motivated application to allsorts, e.g., [digital pregnancy tests](https://twitter.com/Foone/status/1301707401024827392).

### References
<a id="1">[1]</a>
UK Digital Strategy 2017
Department for Digital, Culture, Media & Sport; UK Gov.

<a id="2">[2]</a>
#SMARTER2030 ICT Solutions for 21st Century Challenges (2015)
Global e-Sustainability Initiative

<a id="3">[3]</a>
The energy and emergy of the internet (2011)
Barath Raghavan and Justin Ma

<a id="4">[4]</a>
The Energy Efficiency Benefits and the Economic Imperative of ICT-Enabled Systems (2015)
In: ICT Innovations for Sustainability
Springer International Publishing

<a id="5">[5]</a>
Anders Andrae and Tomas Edler (2015)
On Global Electricity Usage of Communication Technology: Trends to 2030.

<a id="6">[6]</a>
Casamayor, J.L., Su, D. and Ren, Z. (2018)
Comparative life cycle assessment of LED lighting products.
Lighting Research & Technology

<a id="7">[7]</a>
Ran Liu et al. (2019)
Impacts of the digitaltransformation on the environment and sustainability.
Technical report, Oko‑Institut e.V., December2019

<a id="8">[8]</a>
J. Chabarek et al. (2008)
Power Awareness in NetworkDesign and Routing.
The 27th Conference on Computer Communications, IEEE

<a id="9">[9]</a>
Roberto Bruschi et al. (2014)
Green extension of OpenFlow.
The 26th International Teletraffic Congress, IEEE

<a id="10">[10]</a>
Frederic Giroire et al. (2014)
Optimizing rule placement in software‑defined networks for energy‑aware routing.
The Global Communications Conference, IEEE

<a id="11">[11]</a>
Joel Jaeggli (2014)
Energy Management (EMAN) Applicability Statement