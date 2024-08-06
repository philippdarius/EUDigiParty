The EUDigiParty data set supports researchers interested in investigating digital communication activities by political parties in Europe by providing an extensive list of parties’ social media accounts on major digital platforms as of June 2024. The data is valuable for researchers in the fields of political communication, political science, political sociology, and computational social science to inspect party dynamics in Europe from a comparative perspective. The data set also includes identifiers from the Partyfacts database [Version 2023] to enable linking the EUDigiParty data with existing data sets on political parties or country-level data in the European Union.


The EUDigiParty data set: The digital campaigning presence of 401 political parties during the European Parliament election 2024 including websites and social media handles on Facebook, Instagram, TikTok, X/Twitter, and YouTube
Philipp Darius∗ Wiebke Drews† Andreas Neumeier ‡ Jasmin Riedl § August 6, 2024
Please cite as:
Darius, Philipp; Drews, Wiebke; Neumeier, Andreas and Jasmin Riedl. 2024. The EUDigiParty data set: The digital campaigning presence of 401 political parties during the European Parlia- ment election 2024 including websites and social media handles on Facebook, Instagram, TikTok, X/Twitter, and YouTube. DOI: 10.7910/DVN/U6UWPN. Harvard Dataverse. Version 1. August 6, 2024.
 ∗Center for Digital Governance, Hertie School, Berlin, Germany. Contact: darius@hertie-school.org
†Department of Social Sciences and Public Affairs, University of the Bundeswehr Munich, Germany. Contact: wiebke.drews@unibw.de
‡Department of Social Sciences and Public Affairs, University of the Bundeswehr Munich, Germany. Contact andreas.neumeier@unibw.de
§Department of Social Sciences and Public Affairs, University of the Bundeswehr Munich, Germany. Contact jasmin.riedl@unibw.de
1

1 Acknowledgements
We greatly appreciate the excellent research assistance provided by Alexander Berghaus, Korbinian Etterer, Helene Glatz, Marius Heimes, and Bastian Rötzer from the University of the Bundeswehr Munich. The work presented has benefited from funding from dtec.bw - Center for Digitalization and Technology Research of the German Bundeswehr as part of the research project SPARTA and funding by the Center for Digital Governance at the Hertie School. Dtec.bw is funded by the European Union - NextGenerationEU. We are also grateful to our colleagues from the EU&I project EU&I, developed by the EUI in collaboration with the University of Lausanne and Lucerne, for sharing the party lists for the EU2024 before their release, and colleagues from the CamforS project for data exchange, which helped to improve the completeness of our dataset.
2 Introduction
Digital communication on social media platforms has become an essential ingredient of political campaigns. While scholars for long considered European elections second order elections, this may be changing in the future (Gattermann, de Vreese, & van der Brug, 2021; Reif, Schmitt, & Norris, 1997). The 2024 European parliamentary elections underlined an increasing electoral support for radical and Eurosceptic parties. Thereby, these parties are leveraging social media, particularly through platforms like TikTok, to engage with voters, especially younger audiences (Albertazzi & Bonansinga, 2024; González-Aguilar, Segado-Boj, & Makhortykh, 2023).
This data set supports researchers interested in the investigation of digital communication ac- tivities by political parties in Europe by providing an extensive list of parties’ social media accounts on major digital platforms as of June 2024. The data is valuable for researchers in the fields of political communication, political science, political sociology, and computational social science to inspect party dynamics in Europe from a comparative perspective. The data set also includes identifiers from the Partyfacts database [Version 2023] (Bederke, Döring, & Regel, 2023) to enable linking the EUDigiParty data with existing data sets on political parties or country-level data in the European Union. To investigate populist or opposition-government dynamics the data set can, for instance, be linked to the PopuList data set 3.0 (Rooduijn et al., 2023, 2024) or the ParlGov database. Our data collection shows that a majority of European parties have adopted social media as communication channels for their digital campaigning efforts.
3 Data collection
As a starting point, we used a list of European party names running in the 2019 and 2024 European elections provided by the EU&I project (Ferreira da Silva, Reiljan, Cicchi, Trechsel, & Garzia, 2023; Reiljan, da Silva, Cicchi, Garzia, & Trechsel, 2020). Based on this list, we thoroughly searched for party names on selected social media platforms. If no relevant results were found, we also searched for the party names, abbreviations, and platform names via online search engines. Finally, we cross-checked our results with a list of social media accounts provided by the CamforS project.
Table 1 shows an overview of the number of parties per platform in the final data set. Addition- ally, we linked the Partyfacts-Identifier (Bederke et al., 2023) to facilitate further analysis. In total the EUDigiParty dataset contains data on 401 European parties. Facebook is used by 92.77 % of the parties in our dataset whereas TikTok is only used by 43.89% of the parties in the EUDigiParty
1

dataset. Instagram, X/Twitter and YouTube are used by roughly 80% of European parties in our dataset. More details on the variables can be found in the Codebook in Table 2. Of the 401 parties in EUDigiParty, 203 are also part in the most recent Partyfacts data and can be linked easily via the Partyfacts-ID included in the EUDigiParty data set.
Facebook Instagram TikTok X/Twitter YouTube
372 327 176 322 323 92.77 81.55 43.89 80.3 80.55
Table 1: Social media handles included per platform for N=401 European parties and proportion of parties using social media (in percent)
4 Data and Variables
Table 2 describes the variables of the EUDigiParty data set. The data set entails country and party information, links to Wikipedia pages and party webpages as well as the parties’ social media account handles on major digital platforms. Additionally, the data set includes the Partyfacts identifier to link the data with other party or country-level data. The data set is envisioned to enable researchers to collect data from party webpages and Wikipedia pages via scraping and data on party accounts on social media platforms via platforms’ API accesses.
We plan to extend the data set by including LinkedIn handles but could not ensure the same level of validation as for the other platforms for which we double-checked each account and compared with lists of colleagues. Thus, we plan to release a second version including LinkedIn handles and vote shares in the 2019 and 2024 European elections.
In conclusion, the data collection reveals that a significant proportion of European parties actively utilize social media for digital campaigning, with Facebook as the most adopted social medium and TikTok emerging as a relatively new platform, though its adoption is roughly half that of more established social media channels.
      2

 Variable Name
COUNTRY COUNTRY_CODE PARTYFACTS_ID ABBREVIATION PARTY_NAME_ENGLISH PARTY_NAME FOUNDED
PERSON
WIKIPEDIA
WEBSITE_NATIONAL WEBSITE_NATIONAL_SUBPAGE_EU WEBSITE_EU WEBSITE_EUGROUP_SUBPAGE EU_GROUP
TWITTER_NATIONAL FB_NATIONAL
INSTA_NATIONAL TIKTOK_NATIONAL TIKTOK_NAT_DISPLAY_NAME YT_NAT_BIO_HANDLE
YT_NAT_ID
TWITTER_EU
FB_EU
INSTA_EU
TIKTOK_EU TIKTOK_EU_DISPLAY_NAME YT_EU_BIO_HANDLE
YT_EU_ID
Description
Country of the party
Country code (0 for EU-level parties)
Unique identifier as per Partyfacts
Party abbreviation on Wikipedia and Partyfacts English translation of party name
Party name in national language
Year of the party’s foundation
This is an individual candidate, not a party
Link to English Wiki page, if present
Link to national website
Link to EU subpage on national website
Link to EU website
Link to subpage of EU parliamentary group
EU parliamentary group a party belongs to (2019-2024) National Twitter account
National FB account
National Instagram account
National TikTok account
National TikTok display name
National YouTube Handle (starting with "@")
National YouTube ID
European Twitter account
European Facebook account
European Instagram account
European TikTok account
European TikTok display name
European YouTube Handle (starting with "@") European YouTube ID
                                                         Table 2: Description of EUDigiParty variables
3

References
Albertazzi, D., & Bonansinga, D. (2024, July). Beyond anger: the populist radical right on TikTok. Journal of Contemporary European Studies, 32(3), 673–689. Retrieved 2024-08-01, from https://doi.org/10.1080/14782804.2022.2163380 (Publisher: Routledge _eprint: https://doi.org/10.1080/14782804.2022.2163380) doi: 10.1080/14782804.2022.2163380
Bederke, P., Döring, H., & Regel, S. (2023, December). Party Facts – Version 2023. Harvard Dataverse. Retrieved 2024-07-30, from https://dataverse.harvard.edu/dataset.xhtml ?persistentId=doi:10.7910/DVN/TJINLQ doi: 10.7910/DVN/TJINLQ
Ferreira da Silva, F., Reiljan, A., Cicchi, L., Trechsel, A. H., & Garzia, D. (2023, January). Three sides of the same coin? comparing party positions in VAAs, expert surveys and manifesto data. Journal of European Public Policy, 30(1), 150–173. Retrieved 2024-08-01, from https://doi.org/10.1080/13501763.2021.1981982 (Publisher: Routledge _eprint: https://doi.org/10.1080/13501763.2021.1981982) doi: 10.1080/13501763.2021.1981982
Gattermann, K., de Vreese, C. H., & van der Brug, W. (2021, November). Introduction to the special issue: No longer second-order? Explaining the European Parliament elections of 2019. Politics , 41 (4), 423–432. Retrieved 2024-08-01, from https://doi.org/10.1177/ 02633957211035096 (Publisher: SAGE Publications Ltd) doi: 10.1177/02633957211035096
González-Aguilar, J. M., Segado-Boj, F., & Makhortykh, M. (2023, May). Populist Right Par- ties on TikTok: Spectacularization, Personalization, and Hate Speech. Media and Commu- nication, 11(2), 232–240. Retrieved 2024-08-01, from https://www.cogitatiopress.com/ mediaandcommunication/article/view/6358 doi: 10.17645/mac.v11i2.6358
Reif, K., Schmitt, H., & Norris, P. (1997). Second-order elections. European Jour- nal of Political Research , 31 (1-2), 109–124. Retrieved 2024-08-01, from https:// onlinelibrary.wiley.com/doi/abs/10.1111/j.1475-6765.1997.tb00768.x (_eprint: https://onlinelibrary.wiley.com/doi/pdf/10.1111/j.1475-6765.1997.tb00768.x) doi: 10.1111/ j.1475-6765.1997.tb00768.x
Reiljan, A., da Silva, F. F., Cicchi, L., Garzia, D., & Trechsel, A. H. (2020, August). Lon- gitudinal dataset of political issue-positions of 411 parties across 28 European countries (2009–2019) from voting advice applications EU profiler and euandi. Data in Brief, 31, 105968. Retrieved 2024-07-30, from https://www.sciencedirect.com/science/article/ pii/S2352340920308623 doi: 10.1016/j.dib.2020.105968
Rooduijn, M., Pirro, A., Halikiopoulou, D., Froio, C., Kessel, S. v., Lange, S. d., ... Taggart, P. (2023, June). The PopuList 3.0. Retrieved 2024-07-30, from https://osf.io/2ewkq/ (Publisher: OSF) doi: 10.17605/OSF.IO/2EWKQ
Rooduijn, M., Pirro, A. L. P., Halikiopoulou, D., Froio, C., Kessel, S. V., Lange, S. L. D., ... Taggart, P. (2024, July). The PopuList: A Database of Populist, Far-Left, and Far-Right Parties Using Expert-Informed Qualitative Comparative Classification (EiQCC). British Journal of Political Science , 54 (3), 969–978. Retrieved 2024-07-30, from https://www.cambridge.org/core/journals/british-journal-of-political -science/article/populist-a-database-of-populist-farleft-and-farright -parties-using-expertinformed-qualitative-comparative-classification-eiqcc/ EBF60489A0E1E3D91A6FE066C7ABA2CA doi: 10.1017/S0007123423000431
4
