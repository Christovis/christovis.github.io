+++
title = "Climate Discourse in Internet Standards Organizations"
date = "2021-12-08"
+++

<!-- Setting the stage for ICT -->
Information and communications technology (ICT) has played an important role in promoting the transition of society, technology, and economy from the industrial to the information era. Now, our society has to transform to minimise our environmental impact to ensure sustainable future (variously denoted as post-anthropocenic, -cthulucenic, or -capitalocenic , -eurocene epoch). This transformation is imagined to be dependent on and driven by the ICT. Reason being is, that ICT is said to increase the energy efficiency of the economy in general, which currently wastes appr. 86% of the produced energy [[3]](#3). For the energy sector specifically, it would enable a distributed and decentralised energy networks, which would shorten power transmission routes, decrease energy waste, and reduce greenhouse gas (GHG) emissions.


<!-- Need to improve ICT -->
If the ICT sector is to play such a pivotal role in the energy transition, it will take on a significant burden to reduce it's own energy consumption and GHG emissions. While it currently contributes 2.1-3.9% to the total GHG emission of our population (C. Freitag et al 2021), it is projected to dramatically increase within this decade: using 21% of global electricity by 2030 in the expected case, with an 8% or 51% share in the best and worst cases respectively [1]. The most significant trend along this projection, regardless of scenario, is that the energy consumption decreases in consumer devices and increases in networks and data centres. The transformative potential of 5G, on the energy sector specifically and the economy and society in general, puts the Internet infrastructure at the centre of discussions about sustainable development and begs for in depth and cross-disciplinary examination.


<!-- Introducing SDOs -->
In this short article, I want to explore how internet standards-developing organisations (SDO) have so far attended to the climate emergency. While not all Internet governance practices unfold in standard-setting institutions, these bodies are focus points for coordination, and a place where many of the actors that produce the Internet, and exercise infrastructural power, meet. They pose as a space for self-regulated fora and bottom-up coordination (Sowell 2012 and ten Oever 2021). There are a number of relevant SDOs who's work on Internet governance and standardisation is done in cooperation with other SDOs and whose focus can evolve into different directions. To simplify this exploration, I will only focus on the principal SDOs engaged in the development of the Internet’s architecture, namely the International Telecommunication Union-Telecommunication Standardisation Sector (ITU-T), 3rd Generation Partnership Project, Internet Engineering Task Force (IETF) and the World Wide Web Consortium (W3C).


<!-- TCP/IP protocol stack -->
Before uncovering the histories of climate thought in the chosen SDOs, let's sketch the essential parts of the Internet to gain a high-level view. The most universal and persistent element of structure and organisation is the network architecture. The architecture defines how sets of protocols are organised, where protocols define how various modules interact. For the current Internet, the architecture design is the TCP/IP protocol stack (also referred to as the hourglass protocol stack). Although in theory each protocol belongs to one layer in the stack, in practice protocols were required that can 'overlay' between different layers. Thus, even though the image of a tidy stack of separate sets of protocols is outdated, I will list it here as it is what we currently have to work with. As a side note, notable research projects that study new architecture designs are SCION, RINA and NDN.

| Layer          | SDO          | Standards
| -------------- | ------------ | ---------------
| 4 Application  | IETF         | HTTP, HTML, MIME, POP, IMAP, SMTP, DNS, SSH
|                | W3C          | HTTP, HTML, XML
|                | ITU-T        | JPEG
| 3 Transport    | IETF         | TCP, UDP, TLS, QUIC
| 2 Internet     | IETF         | IPv4, IPv6, ICMP, ECM, Seamoby
| 1 Network/Link | IEEE         | Ethernet, WiFi
|                | ITU-T        | ISDN, DSL
|                | 3GPP         | 2G/3G/4G/5G

To be clear, Internet protocols in and of themselves contribute very little to the overall environmental harm when compared to the, e.g., physical materiality that needs to be manufactured for the Internet to work. However, they influence directly the interoperability between systems and indirectly the requirements for new physical equipment. A helpful guidance for SDOs on how to address climate change is given by ISO GUIDE 84:2020.


<!-- ITU -->
All five standardisation bodies in the table have and are working towards a sustainable future. The ITU-T is responsible, inter alia, for studying and issuing recommendations on questions regarding telecommunications and information communication technology. Within its [Study Group 5](https://www.itu.int/en/ITU-T/studygroups/2017-2020/05/Pages/default.aspx), which exists since 1997, the focus lies on recommending design methodologies to reduce environmental impacts of ICT. Examples of published standards are ITU-T [L.1200](https://www.itu.int/ITU-T/recommendations/rec.aspx?rec=11638), which specifies direct current interfaces, and ITU-T L.1300, which describes best practices to reduce negative impact of datacenter on climate. The work of ITU-T/SG5 is motivated by their conviction that ICT is a fundamental pillar in the response as they enable "monitoring climate change, mitigating and adapting". Such narrative derives from the belief that the natural environment needs to be managed and that "We can't manage what we can't monitore", to paraphrase the motto of the Planetary Skin Institute set up by Cisco and National Aeronautics and Space Administration (NASA) in 2009 and shut down since then. Thinkers like Benjamin Bratton oppose such narratives, as it imagines the natural environment is something to be policed, that carries the potential to position us as the antecedent enemy of what is to come.

<!-- 3GPP -->
The 3GPP was founded by the European Telecommunications Standards Institute (ETSI). Documented traces of a change in narrative that include not just energy saving incentives for their OPEX (Operational Expenditure), but also a motivation to 'contribute to the protection of our environment and the environment of future generations' ([[3GPP-1]](#3GPP-1)) are starting to show up in 2009 with Release-10. This change is directly driven by operators wanting to create an 'environmental image' of themselves and indirectly by governments wanting to meet national and international treaties on the climate crisis. Since then the focus has been on six different topics:
- Telecommunication management; study on Energy Savings Management (ESM)
- Operations And Management (OAM) aspects of Energy Saving in Radio Networks
- Study impacts on 'User Equipment - Core network' signalling from Energy Saving
- Study on solutions for energy saving within Universal Mobile Telecommunications System (UMTS) Node-Bs
- Study on network energy saving for Evolved Universal Terrestrial Radio Access Network (E-UTRAN)
- Study on Solutions for Global System for Mobile Communications (GSM) / EDGE Base Transceiver Station (BTS) Energy Saving
Furthermore, ETSI itself set up a technical committee for 'Environmental Engineering' (EE), that published its first standard 'Better determination of equipment energy consumption for improved sizing of power plant' in 2007. Generally this technical committee focuses on the environmental and infrastructural aspects for all telecommunication equipment and its environment, including equipment installed in subscriber premises. Since its creation it has published 15 different standards ([[3GPP-2]](#3GPP-2)). This development partially follows from ETSI signing the EC Mandate M/462 in 2010, which carries the objective to enable efficient energy use in fixed and mobile information and communication networks. <!-- TErrestrial Trunked RAdio (TETRA) is a standard by ETSI is recommended as a dependable system for communications in natural disasters (see book on Early Warning Sytems) -->

<!-- W3C -->
The World Wide Web Consortium (W3C) [Sustainable Web Design community group](https://www.w3.org/community/sustyweb/), which exists since 2013 and focuses on "integration of many areas of design and development into an overarching framework to maximise energy efficiency, lowering environmental impact, and raising inclusiveness." Another community group named 'Climate action, environment, resource efficiency and raw materials' which existed for appr. one year until 2016. It was established under the 'Big Data Europe' project, which was part of the European Union's Horizon 2020 Programme. It mainly served the purpose to '[identify the current as well the future Big Data challenges in the Climate domain](https://www.w3.org/community/bde-climate/2015/09/04/summary-of-1st-community-bde-sc5-workshop/)'. The outcomes would then be used to design and realise the ICT infrastructure needed to benefit from big data technologies, maximising the opportunities of the latest European RTD developments, including multilingual data harvesting, data analytics, and data visualisation. Although this community group was only short lived, there are newer and enduring traces of climate thought within W3C community groups, such as in the following:

- https://www.w3.org/community/bde-food/
- https://www.w3.org/community/sustyweb/
- https://www.w3.org/community/webeco/
- https://www.w3.org/community/wwca/

Furthermore in 2019, when W3C's Technical Architecture Group released their ['Ethical Web Principles'](https://www.w3.org/2001/tag/doc/ethical-web-principles/#sustainable) which explicitly states: 'The web must be an environmentally sustainable platform'. These principles have been labelled as 'anticompetitive' within W3C and shows the competition of views within SDOs. A recently erupted debate around W3C efforts to standardise Decentralized IDentifiers (DID), a prominent use case of non-fungible tokens (NFT). It started with the Mozilla Foundation's  [call to review](https://lists.w3.org/Archives/Public/public-new-work/2021Sep/0000.html) W3C's DID v1.0 in September 2021 as:

> "Proof-of-work methods (e.g. blockchains) are harmful for sustainability (s12y). Also as noted by Google, the registry contains methods which rely upon proof-of-work which is wasteful. “Successful” proof-of-work systems waste a staggering amount of electricity world-wide (e.g. Bitcoin consumes more energy than most countries [...]) demonstrating that the more such methods are adopted, the more their energy requirements grow, without any discernible upper bound, which is grossly irresponsible given the global environmental crisis (recent IPCC report [...])."

To which the responds of W3C's DID working group members was:

> - "It seems like a witch hunt", and
> - "This is a blatant political attack on cryptocurrencies and has no place in interoperability specifications for DID Methods.""

None the less, it was agree to included a section on 'Environmental Considerations' in the [current draft](https://w3c.github.io/did-imp-guide/#environmental-considerations).


<!-- IETF -->
The Internet Engineering Task Force (IETF) is among the most open and transparent Internet SDOs. A clear example of IETF's influence is given by its redesign of the IPv4 communication protocol into the improved version IPv6. The redesign does not only solve the problem of IPv4 address exhaustion, but is also claimed to reduce energy usage and increases flexibility towards green networking (e.g., [[7]](#7), [[8]](#8), [[9]](#9), [[10]](#10)). In 2010, the IETF set up the Energy Management working group (EMAN, [[11]](#11)) to create a framework standard that enables monitoring, controlling, and managing of the energy consumption of networking and network-attached devices while still providing sufficient performance to meet service level objectives. Five years later however, the EMAN working group was shut down and has never been reactivated despite remaining problems, e.g., it does not address questions regarding electricity producers and distributors as well as the roll-out of new technologies (e.g., IoT and 5G). But other dimensions through which impacts on climate and ecology can be addressed are present in other working groups that are concerned with, e.g., smart energy, smart grid, and the Internet of Things.

<!-- On the other hand, IETF Eman (Internet Engineering Task Force-Energy Management) studies several MIBs for energy management of network devices in ICT systems for international standardisation actively. These MIBs are based on SNMPs but all drafts by EMAN are caught in the proposal stage (e.g. RFC 7603 which hasn't considered security issues of SNMPs, as the reviewer writes "This necessarily extends to monitoring, and there is certainly a *lot* of information that may be gleaned by an attacker from monitoring power consumption,"). -->

<!-- At present, the proposed energy-efficient methods are usually divided into two classes: one is on device-level, which provides the energy-efficient network devices and terminals; the other is on system-level, which organises the usage of devices and terminals energy-efficiently in a network-wide manner. The energy-efficient routing algorithm belongs to system-level energy saving scheme, which aims to find the most energy-efficient route for users and thus reduce energy consumption when transferring traffic along the route. -->

<!-- Now, the ICT sector is in a similar situations and various 'ICT for Sustainability' ([ICT4S](https://conf.researchr.org/series/ict4s)) and Green IT initiatives have cropped up over the years. -->

<!-- And here, it is worthwhile to dwell on the what this space 'elsewhere' is. However, the observation that decreasing a processes resource intensity does not lead to a decrease in overall consumption, has already been described by Stanley Jevons in his 1865 work "The Coal Question". The so called "Jevons paradox" has since then always gone alongside the pursued to increasing efficiency and economic growth. Taking LEDs as an example, 'elsewhere' has come to be a very large space indeed. Their appr. 60% lower environmental impact than fluorescent luminaire [[12]](#12), and more so their impression of 'advanced technology', has motivated application to allsorts, e.g., [digital pregnancy tests](https://twitter.com/Foone/status/1301707401024827392). -->

<!-- B. Bratton "this in turn may put the design of the *Earth* layer of The Stack in the untenable position of working on behalf of the exceptional emergencies that most threaten the platform's coherency, such that in the decades to come, the self-amplifying logics of ecological governance demand not only geoengineering, but also incredible computational energy capture-and-distribution megastructures far beyond our current capabilities." page 76 -->




<!-- And the systems logical understanding of a geographic, bio-informational, planetary-scale epidermal sensing and computation megastructure as been promoted by many personalities (such as Al Gore, ...), projects (such as the GeoWeb \cite{herring_architecture_1994}, Al Gore's The Digital Earth, Cisco’s Planetary Skin, and NGA’s requirements for On-Demand Geospatial-Intelligence or GEOINT2), and the organisations behind them -->

<!-- The idea of \emph{infrastructural globalism} \cite{edwards_vast_2010} or \emph{The Stack} \cite{bratton_stack_2015}, which describe how the building of technical systems for gathering global data helped create global institutions and ways of thinking globally. -->



<!-- ### Footnote
<a id="ft-1">[ft-1]</a> -->

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


<a id="3GPP-1">[3GPP-1]</a>
https://blog.3g4g.co.uk/2010/10/3gpp-green-activities-energy-saving.html
Published: 05/10/2010
Accessed: 23/02/2022

<a id="3GPP-2">[3GPP-2]</a>
https://www.etsi.org/technologies/environmental-aspects
Published: 2022
Accessed: 23/02/2022
