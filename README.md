# osint-timelines

## Reason

Most IOCs these days are shared without time context, thus analysts wasting time
investigating hit in their envirenment that have been taken place before or even after
an malicious campaign.

Therefore this repository shall give a time context / extract of published reports as CSV files.

There was also a discussion on [Twitter](https://twitter.com/alexanderjaeger/status/1070311545874337792)

To showcase the idea thie repository was created.

## Using

Use the CSV however you want, if you make them a product, please make a reference back.

### Timesketch

All csv files should be ready to be imported directly as CSV into [Timesketch](https://timesketch.org) to enable analysts
use the timelines as an overlay to their internal analysis.

## Structure

Every year has a folder containing a csv per OSINT report.

## header

### mandatory

It was decided to use the mandatory header fields of timesketch to ensure compatibility.

* message
  * String with an informative message of the event
* datetime
  * ISO8601 format
  * Ex: 2015-07-24T19:01:01+00:00
* timestamp_desc
  * String explaining what type of timestamp it is. E.g file created
  * Ex: "Time created"

You need to provide the CSV header with the column names as the first line in the file.

    message,timestamp,datetime,timestamp_desc,extra_field_1,extra_field_2
    A message,1331698658276340,2015-07-24T19:01:01+00:00,Write time,foo,bar
    ...

### optional

You can add as much optional fields as you want. E.g. attribution if it is attributed to a certain group / campaign.

It is also recommended to provide a source field which contains the link to the source of the data point.

### Why not format xyz

There are already a good amount of formats out there to cover various aspects of threat intel.
For timelines in particular, there is no well established standard / format, so csv seems to be the way to go.
It is usable in Office as well as various other tools to be easily imported / exported.

## How to contribute

Every contribution is highly welcome. If you come across a OSINT report that is not yet covered, feel free to make it a csv.

* open an issue to cover an new report
* provide a csv file for a report

## 2021

| Date   | Title           | Added  | Link  |
| ------------- |-------------| -----|---|
| 2021-07-17|Forensic Methodology Report: How to catch NSO Group’s Pegasus|Yes|[Link](https://www.amnesty.org/en/latest/research/2021/07/forensic-methodology-report-how-to-catch-nso-groups-pegasus/)

## 2019

| Date   | Title           | Added  | Link  |
| ------------- |-------------| -----|---|
| 2019-01-10|Big Game Hunting with Ryuk: Another Lucrative Targeted Ransomware|Yes|[Link](https://www.crowdstrike.com/blog/big-game-hunting-with-ryuk-another-lucrative-targeted-ransomware/)
| 2019-01-30|The Double Life of SectorA05 Nesting in Agora (Operation Kitty Phishing)|Yes|[Link](https://threatrecon.nshc.net/2019/01/30/operation-kitty-phishing/)
| 2019-02-22|New BabyShark Malware Targets U.S. National Security Think Tanks|Yes|[Link](https://unit42.paloaltonetworks.com/new-babyshark-malware-targets-u-s-national-security-think-tanks/)
| 2019-02-27|APT27 A Peek into BRONZE UNION’s Toolbox|Yes|[Link](https://www.secureworks.com/research/a-peek-into-bronze-unions-toolbox)
| 2019-03-29|Exodus: New Android Spyware Made in Italy|Yes|[Link](https://securitywithoutborders.org/blog/2019/03/29/exodus.html)
| 2019-05-15|Winnti: More than just Windows and Gates|Yes|[Link](https://medium.com/chronicle-blog/winnti-more-than-just-windows-and-gates-e4f03436031a)

## 2018

| Date   | Title           | Added  | Link  |
| ------------- |-------------| -----|---|
| 2018-12-29|Parsing the Cozy Bear LNK File|Yes|[Link](http://windowsir.blogspot.com/2018/12/parsing-cozy-bear-lnk-file.html)
| 2018-12-21| OVERRULED: Containing a Potentially Destructive Adversary | yes |[Link](https://www.fireeye.com/blog/threat-research/2018/12/overruled-containing-a-potentially-destructive-adversary.html)
| 2018-12-19| When Best Practice Isn’t Good Enough: Large Campaigns of Phishing Attacks in Middle East and North Africa Target Privacy-Conscious Users | yes |[Link](https://www.amnesty.org/en/latest/research/2018/12/when-best-practice-is-not-good-enough/)
| 2018-12-05| Flash 0day + Hacking Team RAT: Activities of Exploiting Latest Flash 0day Vulnerability and Correlation Analysis | yes |[Link](https://ti.360.net/blog/articles/flash-0day-hacking-team-rat-activities-of-exploiting-latest-flash-0day-vulnerability-and-correlation-analysis-en/)
| 2018-12-03| Analysis of cyberattack on U.S. think tanks, non-profits, public sector by unidentified attackers |yes | [Link](https://cloudblogs.microsoft.com/microsoftsecure/2018/12/03/analysis-of-cyberattack-on-u-s-think-tanks-non-profits-public-sector-by-unidentified-attackers/)
| 2018-11-29| Attack_Pakistan_By_Exploiting_InPage |yes |[Link](https://ti.360.net/blog/articles/analysis-of-targeted-attack-against-pakistan-by-exploiting-inpage-vulnerability-and-related-apt-groups-english/) |
| 2018-11-19| Not So Cozy: An Uncomfortable Examination of a Suspected APT29 Phishing Campaign |yes|[Link](https://www.fireeye.com/blog/threat-research/2018/11/not-so-cozy-an-uncomfortable-examination-of-a-suspected-apt29-phishing-campaign.html)
| 2018-11-16| New Strain of Olympic Destroyer Droppers |yes|[Link](https://research.checkpoint.com/new-strain-of-olympic-destroyer-droppers/)
| 2018-09-13| APT10 Targeting Japanese Corporations Using Updated TTPs |yes|[Link](https://www.fireeye.com/blog/threat-research/2018/09/apt10-targeting-japanese-corporations-using-updated-ttps.html)
| 2018-06-19| Olympic Destroyer is still alive|Yes|[Link](https://securelist.com/olympic-destroyer-is-still-alive/86169/)

## 2017

| Date   | Title           | Added  | Link  |
| ------------- |-------------| -----|---|
| 2017-04-??| Operation Cloud Hopper APT10 | Yes |[Link](https://www.pwc.co.uk/issues/cyber-security-data-privacy/insights/operation-cloud-hopper.html)

## Links

Some good sources of OSINT reports to be covered:

* [github/APT_CyberCriminal_Campagin_Collections](https://github.com/CyberMonitor/APT_CyberCriminal_Campagin_Collections/)
