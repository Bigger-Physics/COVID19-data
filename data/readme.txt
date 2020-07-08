The data of China are collected from publicly available official reports of case investigations, which were performed by investigators in the corresponding centers for
disease control and prevention in each province. In general, the official reports are published on the official websites of Provincial Public Health Commissions (e.g., http://wsjk.tj.gov.cn), the official social media accounts of governmental or public health institutions (e.g, https://wx.hebnews.cn/xcgj/), or other news websites(e.g., https://www.sohu.com). The data of Singapore are collected from publicly available official reports of the Ministry of Health of Singapore (https://www.moh.gov.sg/covid-19/past-updates). 

A description of the fields in the database is shown as follows.

ID: Unique identifier for reported case. It includes the information of Province and City, e.g. Hebei-Tangshan-5. Therefore, the data can also be used to investigate the evolution of Covid-19 in each city.

age:Age of the case reported in years. When not reported, null is used.
sex: Sex of the case. When not reported, null is used.

city of being infected: City/country where the case may be exposed. 

City of being officially reported: City/country where the case was first reported. Note that imported cases will be assigned to the city/country in which confirmation occurred, rather than the City/country where the case may be exposed.

Time of being infected: Date when a case with no travel history may be infected. Note L and R indicates the earliest possible infection date and the latest possible infection date. Specific dates are reported as YYYY/MM/DD.

Time of leaving the infecting city: Date the imported case left the place of residence, and travel to the reporting city.

Time of arriving at the reporting city: Date the imported case arrived at the reporting city.

Time of going to the infecting city: Date leaving the reporting city to the infected city for travel.

Time of returning to the reporting city: Date returning to the reporting city after the trip.


Time of symptom onset: Date when the reported case began to show symptoms. When not reported, the date are recorded as YYYY/MM/DD-, where YYYY/MM/DD is the time of being officially reported.

Time of being officially reported: Date when the reported case was confirmed as having COVID-19. When not available in online report, the date are recorded as YYYY/MM/DD+, where YYYY/MM/DD is the time of symptom onset.

Infected by: IDs who the reported case was possible infected by.

Generation number: Generation of reported case. For example, imported cases are marked as $0$ generation. Cases infected directly by the imported cases or had contacted guys from Hubei recently are marked as $1$ generation. Cases infected by the first-generation cases are marked as  $2$ generation cases and similarly for higher-generation cases. In particular, if the infector is unknown, the generation is defined as follows. If the reported case is the close contacts of non-imported case, he is marked as $2+$ generation. In particular, in Singapore data, if case was known to be assigned in some clusters, he is also marked as $2+$ generation. non-imported case is marked as $1+$ generation. Correspondingly, their infectees are marked as $(n+1)+$ generations.

Finally, the database of China contained 4111 records from January 20th, 2020 to February 29th, 2020. There are 509 transmission pairs. In addition, the Singapore dataset comprised 939 (97.2\%) confirmed cases from the date of the initial case on January 23, 2020 until March 31, 2020.
