# Medicare-and-Medicaid-Analysis-on-Health-Charges
# Cleaning and Analyzing data in Power query, Power BI and SQL 
# Introduction
This project is a personal related project. I analyzed a dataset from CMS's Medicare Provider Analysis and Review (MEDPAR) inpatient data file based on fiscal year. The dataset contained 163,065 rows and 12 columns. The following variables are included in the detailed Public Use File (PUF) data file:

a) DRG Definition: This is the code and description identifying the MS-DRG (Medicare Severity Diagnosis Related Group). MS-DRG are a classification system that groups similar clinical conditions (diagnosis). 

b) Provider Id: This is the CMS  certification number (CCN) assigned to medicare certified hospital facility.

c) Total discharges: The number of discharges billed by the provider for inpatient hospital services

d) Average covered charges: The provider's average charge for services for all discharges.

e) Average total payments: The average total payments to all providers including co-payment and deductible amounts that the patient is responsible for.

f) Average medicare payment: The average amount that medicare pays to the provider for medicare's share of the MS-DRG.

The aim of this research is to analyse health care charges across all provider states. 
#  Data Profiling, Data Aggregation and Data Transformation
After importing my data into power query, I checked for the validity of my data using column distribution, quality and profiling and removed columns not necessary for my analysis. I also made sure my columns were in the right data type.
![IMG_1511](https://github.com/OlotoDamilola/Medicare-and-Medicaid-Analysis-on-Healthcare-Charges/assets/109422215/a248bef6-ab6d-48f3-b338-91880d0bb7cb) 
The dataset were duplicated and modified to make it more suitable for analysis. DRG's were grouped by category to obtain the summarized average of total payments and discharges. Provider's name, provider's region and provider's state were also grouped to category to obtain the average payment 
![IMG_1509](https://github.com/OlotoDamilola/Medicare-and-Medicaid-Analysis-on-Healthcare-Charges/assets/109422215/98863df9-911a-4ef5-8346-88e4bd36dc4d) 
#  Data Analysis & Visualizations
1) The Uva Health Sciences Center is situated in Charlottesville, Virginia, which is in the country's South Atlantic region. The average payment is $50,552.61 at Uva Health Sciences Center, with Vail Valley Medical Center coming in second at $42.446.71. The top 10 high providers were dominated by California providers. Memorial Hospital Los Banos, Standard Hospital, and UCSF Center are the providers, with average payments of $25,592.87, $24,354.78 & $23,364.71 per provider, respectively. The "460-Spinal Fusion Except Cervical w/o mcc" procedure at Pinnacle Hospital in Crown Point, Indiana, cost a fortune and caused a significant increase in the average total payment, pushing it into fifth place among providers.
![IMG_1745](https://github.com/OlotoDamilola/Medicare-and-Medicaid-Analysis-on-Healthcare-Charges/assets/109422215/be76a05f-a3e3-4170-b1c0-2a1a33514433)

2) All regions have different average total payments, with some regions having substantially higher payments than others. There were 306 regions analyzed. In California, 23 out of 24 regions appeared in the top half of high average payments. Californian regions dominated the top 10 average payment as well. San Mateo County, California has the highest average total payment of $17,024.48. San Mateo County has a total of 6 hospitals and a 278 discharges of inpatient overall. San Francisco, Salinas, San Jose, Almeida County, and Contra Costa County are other California regions in the top 10, with average total payments of $15,614.75, $15,494.01, $15,334.97, $14,578.75, and $14,129.07, respectively.The majority of these areas are in the state's northern section and because of their large population numbers, the average total payment there tends to rise. After San Mateo County, Bronx, New York comes in second with an average payment of $16,521.30. On the other hand, Dubuque, Iowa has the least average payment at $6,521.39 having a total of 2 hospitals and 110 discharges overall.
![IMG_1744](https://github.com/OlotoDamilola/Medicare-and-Medicaid-Analysis-on-Healthcare-Charges/assets/109422215/3b42b254-d117-459c-aefd-eda9ef1b19c8) 

3) Alaska is located near the northwest extremity of North America. This state only has one region with a total of 9 hospitals, which is quite few and just a little bit more than Delaware, the District of Columbia, North Dakota, and Vermont. With a average total payment of $14,572.39, Alaska has the highest average of all the states. The fact that there aren't enough hospitals in Alaska may be the cause of the high average payment. At $12,998.03, District of Columbia (DC) ranks second among states with high average payments, just ahead of third-placed Hawaii ($12,775.74). Hawaii and the District of Columbia both had few hospitals. Although there are many hospitals in California (295) and New York (161) in various regions, the average total payment is fairly expensive at $12,629.69 and $11,795.49, respectively.
![IMG_1742](https://github.com/OlotoDamilola/Medicare-and-Medicaid-Analysis-on-Healthcare-Charges/assets/109422215/8a695c8e-5f37-42a5-b8a9-434914589dcc)

4) With 27,592 discharges, Good Samaritan Hospital in San Jose, California, has the most inpatient discharges of any hospital. 8 other hospitals are located in San Jose, California. With 25,828 discharges, Florida Hospital in Orlando, Florida comes in second. The city of Orlando, Florida, has 27 other hospitals. Good Samaritan Hospital and Florida Hospital are the only providers who registered above 20,000 discharges. Hospitals registering above 10,000 discharges are mostly from California, New York and Florida. For example, Baptist Medical Center in Jacksonville, Florida (18,208), Mercy Hospital in Bakersfield, California (12,829), New York-Presbyterian Hospital in Manhattan, New York (16,834), Montefiore Medical Center in Bronx, New York (12,204), St Joseph Hospital in Redding, California (10,883) e.t.c.
![IMG_1727](https://github.com/OlotoDamilola/Medicare-and-Medicaid-Analysis-on-Healthcare-Charges/assets/109422215/55904410-8c0e-486f-9949-b7e989dc2f9b)

5) High resource conditions could include the severity of the sickness, level of demand for comprehensive care management and degree of impairment. Septicemia or Severe Sepsis has the most expensive charges to cover its treatment or diagnostic services. Although Spinal Fusion has the most discharges overall accumulating 65,997 discharges. Spinal Fusion is also a complex condition with average covered charges of $92,568.28. Other high resource DRG in the top 10 according to their discharges include, Infectious and Parasitic diseases (39,482), Major Joint Replacement or Reattachment of Lower Extremity (18,714), Other Vascular Procedures (34,222).
![IMG_1746](https://github.com/OlotoDamilola/Medicare-and-Medicaid-Analysis-on-Healthcare-Charges/assets/109422215/a09b3dd9-8632-4316-b95e-732f1d5028e2)

6) It is hardly surprise that the top four states with the greatest discharges are California, Florida, New York, and Texas. Florida has the highest discharge of 536,859  with Texas being second at 479,939. Texas has a greater discharge rate than California, with a difference of 4,960. Also, the fact that Alaska records the fewest discharges is not surprising given the state's tiny number of hospitals. Alaska was successful in documenting 6,142 patient discharges. There were fewer than 20,000 discharges in Idaho, North Dakota, Montana, Hawaii, Vermont, and Wyoming. Additionally, despite having more hospitals, some states nevertheless record lower discharge rates. For example, Nebraska has a total of 23 hospitals and accumulated 39,799 discharges while Nevada has a total of 21 hospitals and accumulated 42,600 discharges.

   ![IMG_1726](https://github.com/OlotoDamilola/Medicare-and-Medicaid-Analysis-on-Healthcare-Charges/assets/109422215/d2f5e586-0e0c-43f6-98c8-ea9883913fc0)

7) States guarantee access to high-quality treatments for those with Medicare and Medicaid. In the meantime, Medicare payments differ between states. Alaska receives the largest Medicare payment, averaging $12,958.97, followed by the District of Columbia, which receives $11,811.97. Hawaii, Wyoming, and Vermont, states with fewer hospitals and discharges, were among the top 10 states with the highest average Medicare payments. California receives average of $11,494.38 from Medicare, while New York receives $10,620.74. Florida, the state with the highest discharges, ranked 36th in average Medicare payments with a $7,667 payment.

8) All states in the top 10 high Medicare payment were all made by top 10 high average total payment. However, some states changed their positions. As stated earlier, Alaska has the highest average total payment. Other states with high average charges include; District of Columbia ($12,978.03), California ($12,629.67), Maryland ($12,608.95), Hawaii ($12,775.74), New York ($11,795.49), Vermont ($11,766.30), Connecticut ($11,365.45), New Jersey ($10,678.99), Wyoming ($11,398.49).
![IMG_1725](https://github.com/OlotoDamilola/Medicare-and-Medicaid-Analysis-on-Healthcare-Charges/assets/109422215/66896576-b910-4779-8fbd-499c26ef7edf)

9) As stated earlier when analyzing the the high resource conditions. Septicemia is the most expensive at $44,259.49 total payments and  $41,899.43 Medicare payments. Infectious and Parasitic Diseases comes in second place at average total payment of $40,315.96 and Medicare payment of $37,818.74. Hip & Femur Procedures Except Major Joint is in the 10th position of total payment of $20,984.37 and Medicare payment of $19,616.95. There was an average of $2,253.30 between the total payment and  Medicare payment of the high resource conditions.
![IMG_1743](https://github.com/OlotoDamilola/Medicare-and-Medicaid-Analysis-on-Healthcare-Charges/assets/109422215/d9a186ea-67e5-49c4-aed0-5c776c4bd5ae)

# Recommendations
a) California's Northern areas needs to be managed considering the average total payment there is $15,481.24

b) More medical facilities should be developed in Alaska to reduce cost of healthcare

c) Since hospitals in Florida and California register more patient discharges, better facilities and medical equipment should be provided to further improve patient care

d) The case of spinal fusion seems to be widespread among providers, better tools should be available to modify medical treatment

e) Florida's medicare payment should be increased to better serve the state's citizens

