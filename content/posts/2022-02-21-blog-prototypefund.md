+++
title = "BigBang - Für ein transparenteres und rechenschaftspflichtiges Internet"
date = "2022-02-21"
+++

> Blog post is also hosted by Prototype Fund [here](https://demoweek.prototypefund.de/projects/03-bigbang.html).

Jedes Mal, wenn man das Internet benutzt, sei es, um mit Verwandten in Kontakt zu bleiben oder Nachrichten aus aller Welt zu lesen, verlässt du dich auf die Arbeit von Normgremien, um ein schnelles, sicheres und genaues Übermitteln von Webseiten, Videos und Telefonsignalen zu garantieren. Es gibt eine Vielzahl von unterschiedlichen regionalen und globalen Normgremien, die Standards und Protokolle für das Internet definieren. Zwei der wichtigsten Normgremien sind die '[Internet Engineering Task Force](https://www.ietf.org/)' (IETF) und das '[World Wide Web Consortium](https://www.w3.org/)' (W3C) die zusammen Standards so wie HTML, JPEG, SSH, oder PGP gesetzt haben.

Genauso wie man nicht über die Kabel, Datenzentren oder Antennen nachdenken muss, wenn man im Internet surft, entfaltet sich der enorme Einfluss von Normgremien auf z. B., die Fähigkeit privater Nutzer ihre eigenen Datenströme zu kontrollieren, oftmals unbemerkt im Hintergrund. Auch wenn einige Normgremien offen für die Teilnahme eines jeden sind, werden sie oft von internationalen Konzernen (so wie Ericsson, Qualcomm, Siemens, Nokia, Huawei) dominiert, die für das Internet verantwortlich sind. Das kontrollieren, ob neue Standards gewisse Kriterien erfüllen (auf z. B., die Gewährleistung der Privatsphäre von Nutzern) oder richtig implementiert werden, wird den von privaten Unternehmen dominierten Normgremien selbst überlassen.

Mit BigBang haben wir uns das Ziel gesetzt, die Machtverhältnisse, Intentionen und Motivationen innerhalb der Normgremien offen zu legen und sie somit transparenter und rechenschaftspflichtiger zu machen. Normgremien so wie IETF und W3C veröffentlicht nicht nur einen großen Teil ihrer Berichte und Dokumente, sondern auch Aufzeichnung von Treffen, Telefonkonferenzen und Mailinglisten auf ihren Webseiten. Diese Archive bieten Forschern eine einzigartige Gelegenheit, die Prämissen von den Entscheidungen, die innerhalb von Normgremien getroffen werden, zu untersuchen. Insbesondere Mailinglisten sind der Ort, an dem sich die vielfältigen Schichten der Normgremien widerspiegeln und Entscheidungsfindungen sichtbar gemacht werden. Des Weiteren besitzen sie die folgenden Vorteile:
- Mailinglisten sind strukturiert: Sie selber besitzen eine standardisierte Struktur, die seit den frühen Anfängen des Internets beihalten wurde. Somit machen Kopfzeilen Metadaten (z. B. Absender und Zeitstempel) leicht zugreifbar, was verschiedene Arten der Klassifizierung und Analyse unterstützt.
- Mailinglisten sind bereichsübergreifend: Eine Vielzahl von unterschiedlichen Fachgruppen tauschen sich innerhalb thematisierter Mailinglisten aus. Dies ermöglicht es Forschern somit, die Interaktion (z. B. Zusammenarbeit und Reibungspunkte) zwischen den Fachgruppen untersuchen.
- Mailinglisten sind relational: Sie liefern Informationen über Beziehungen zwischen Akteuren (z. B. wer adressiert wen), was es Forschern ermöglicht zu sehen, wer an Entscheidungen teilnimmt oder ausgelassen wird.
- Mailinglisten sind mehrdimensional: Indem sie viele verschiedene Facetten besitzen, ermöglichen sie eine Reihe an statistischen Methoden so wie Häufigkeitsverteilung, Diskurs-, Zeitreihen- und Netzwerkanalyse.

Um BigBang zugänglich zu machen, haben wir die weit verbreitete Programmiersprache Python verwendet, eine Befehlszeilenschnittstelle erstellt und Jupyter notebooks geschrieben die Tutorien beinhalten.

Der Anwendungsablauf von BigBang ist in drei Phasen unterteilt. Erstens, muss man angeben auf welche Mailinglisten zugegriffen werden soll. Bigbang enthält alle bestehenden Mailinglisten von [IETF](https://github.com/datactive/bigbang/blob/main/examples/url_collections/mm.ietf.org.txt), [W3C](https://github.com/datactive/bigbang/blob/main/examples/url_collections/W3C.txt), [3GPP](https://github.com/datactive/bigbang/blob/main/examples/url_collections/listserv.3GPP.txt), [ICANN](https://github.com/datactive/bigbang/blob/main/examples/url_collections/mm.icann.org.txt), und [IEEE](https://github.com/datactive/bigbang/blob/main/examples/url_collections/listserv.IEEE.txt). Such die Mailinglisten in du interessiert bis heraus und kopiere sie in eine Textdatei.

Zweitens, müssen die Mailinglisten heruntergeladen werde. Dies kann man entweder manuell in einem Python Programm machen,
```python
from bigbang.ingress import W3CMailList,

mlist = W3CMailList.from_url(
    name="public-webauthn",
    url="https://lists.w3.org/Archives/Public/public-webauthn",
)
```
oder durch die Befehlszeilenschnittstelle in dem du eine das folgende in ein Terminal/Konsole eintippst:
```bash
$ python3 bin/collect_mail.py -f <Dateipfad zu der Textdatei>
public-webauthn: 100%|#######################################################| 17956/17956 [7:58:47<00:00,  1.60s/it]
www-voice:  34%|######################8                                        | 1408/4128 [38:24<1:16:19,  1.68s/it]
```
Da dies ein Zeitaufwendiges verfahren sein kann für große Mailinglisten (einige Mailinglisten umfassen bis zu 200k E-Mails, wodurch es bis zu 111 Stunden dauern kann, um sie herunterzuladen), arbeiten wir daran, um die Datensätze in einem leichter zugänglichen Format zu teilen, welches die DSGVO Grundsätze berücksichtigt.

Nachdem alle Mailinglisten heruntergeladen wurden, können sie mit ein Par bereitgestellten Funktionen analysiert werden, z. B., das Zählen der gesendeten Nachrichten per Domänenteil
```python
mlist.get_messagescount(
    header_fields=["comments-to"],
    per_address_field="domain",
)
```
oder das Filtern aller Nachrichten mit einer bestimmten Betreffzeile
```python
mlist.crop_by_subject(match="EVS SWG Sessions")
```

Mit fortgeschrittenen Funktionen können Ergebnisse erzielt werden, wie sie in den folgenden Figuren zu sehen sind.

![Communication Network in 3GPP_TSG_RAN_WG5_IOT](/assets/internet_governance/bigbang_communication_network.png?raw=true)
Bild 1: Kommunikationsnetzwerk der 3GPP Mailingliste '[3GPP_TSG_RAN_WG5_IOT](https://list.etsi.org/scripts/wa.exe?A0=3GPP_TSG_RAN_WG5_IOT)'. Violette und dünne Linien deuten auf weniger gesendete Nachrichten hin als rote und dicke Linien. Daraus schlussfolgert, das insbesondere Huawei viele Nachrichten mit Eircsson und Siemens ausgetauscht hat.

![Network centralities in 3GPP_TSG_RAN_WG4_IOT](/assets/internet_governance/bigbang_centralities.png?raw=true)
Bild 2: Von links nach rechts sind die Gradzentralität, Nähezentralität und Zwischenzentralität für verschiedene Domänenteile in der 3GPP '[3GPP_TSG_RAN_WG4_IOT](https://list.etsi.org/scripts/wa.exe?A0=3GPP_TSG_RAN_WG4_IOT)' Mailingliste berechnet. Von den drei Zentralitäten es erkennbar das insbesondere ETSI, ein Partnerprojekt von 3GPP, und die 'China Academy of Telecommunications Technology' (CATT) besonders relevant sind.

![Number of send and received messages by Chinese companies in the 3GPP_TSG_CT_WG4](/assets/internet_governance/bigbang_msgs_send_received.png?raw=true)
Bild 3: Oben ist die Anzahl der pro Jahr gesendeten und unten der empfangenen E-Mails von Chinesischen (farbige Linien) und anderen (graue Linien) Firmen in der 3GPP '[3GPP_TSG_CT_WG4](https://list.etsi.org/scripts/wa.exe?A0=3GPP_TSG_CT_WG4)' Mailingliste zu sehen. Die vertikalen gepunkteten Linien markieren Jahre in denen neue Standards veröffentlicht wurden.


Um eine detailliertest How-To Tutorium zu folgen, haben wir dieses Video für dich erstellt: https://www.youtube.com/watch?v=JWimku8JVqE

BigBang hat bereits aktive Entwickler- und Nutzergruppen bestehend aus AkademikerInnen und AktivistInnen der Zivilgesellschaft und wurde für Projekte der Menschenrechtsorganisation [ARTICLE19](https://www.article19.org/), des '[Center for Democracy and Technology](https://cdt.org/)' (CDT), und des '[Centre for Internet & Society](https://cis-india.org/)' (CIS-India) verwendet. Veröffentlichte Resultate beinhalten unter anderem die Untersuchungsergebnisse von Diversität von ICANN ([[1]](#1)) und in wie weit Menschenrechte von Netzinfrastrukturanbieter berücksichtigt werden ([[2]](#2), [[3]](#3)).


### References
<a id="1">[1]</a>
[ICANN Diversity Analysis](https://cis-india.org/internet-governance/blog/icann-diversity-analysis)
Akriti Bopanna, 2018


<a id="2">[2]</a>
[Public interest, private infrastructure: An analysis of the barriers and drivers for adopting human rights standards in the Internet infrastructure industry](https://www.article19.org/wp-content/uploads/2018/06/HRIA-report-UNGP_5.6.pdf)
ARTICLE 19, 2018


<a id="3">[3]</a>
[Human Rights Due Diligence and Internet Infrastructure](https://www.article19.org/wp-content/uploads/2021/06/A19-and-DIHR-pilot-project-outcome-report_FINAL.pdf)
ARTICLE 19, 2021
