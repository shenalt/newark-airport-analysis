# NewarkAirportScalesInvestigation2026
This repository contains the data and analysis gathered to conduct my investigation into Newark Liberty International Airport scales in conjunction with the New York City News Service and with the support of the Equity Through Data Project at the Craig Newmark Graduate School of Journalism at CUNY and published with NJ Spotlight News. In order to build the datasets, I had to parse out the numbers from the .pdf files sent to me by NJ DCA and input them into a spreadsheet. I double checked the data by cross-referencing the spreadsheet and the emailed documents to ensure accuracy. Once that was done, I was able to analyze the data.  

# Data:
1. newarkInitInspections.csv: The data from the inspection report on every scale examined by the New Jersey Division of Consumer Affairs on tktk given to me by the Division of Consumer Affairs through an OPRA request submitted on June 25, 2025. The data was received on August 5, 2025. The data consists of:

- Initial Scale Inspection Report - Terminal A - Newark Liberty International Airport
- Initial Scale Inspection Report - Terminal B - Newark Liberty International Airport
- Initial Scale Inspection Report - Terminal C - Newark Liberty International Airport

The dataset combines the inspections of each scale at every terminal into one main source containing identifiying information of the scale, what terminal it belongs to, weight test result, overall test result and exact amount of pounds either over or underweighed in total.

2. NewarkReinspection.csv: The data from the re-inspection report conducted by the New Jersey Division of Consumer Affairs on tktk given to me by the Division of Consumer Affairs through an OPRA request submitted on June 25, 2025. The data was received on August 5, 2025. The data consists of:

- Initial Scale Re-Inspection Report - Terminal A - Newark Liberty International Airport
- Initial Scale Re-Inspection Report - Terminal B - Newark Liberty International Airport
- Initial Scale Re-Inspection Report - Terminal C - Newark Liberty International Airport

The dataset combines the re-inspections of each scale at every terminal into one main source containing identifiying information of the scale, what terminal it belongs to, weight test result, overall test result and exact amount of pounds either over or underweighed in total.

# Data Dictionary
1. Sticker Number: Identifiying scale sticker number
2. Serial Number: Identifiying scale serial number
3. Date: Date inspection took place
4. Terminal: Terminal where scale is located
5. Registration #: Identifiying scale registration number
6. isAllPass?: Boolean value based on whether the scale passes every weighted test or not
7. Results: Inspection result
8. Type of Scale: Scale's operable weight range
9. Test 0 lbs: Boolean value based on whether the scale passed the 0 lbs test or not
10. Test 50 lbs: Boolean value based on whether the scale passed the 50 lbs test or not
11. Test 100 lbs: Boolean value based on whether the scale passed the 100 lbs test or not
12. Test 150 lbs: Boolean value based on whether the scale passed the 150 lbs test or not
13. Test 200 lbs: Boolean value based on whether the scale passed the 200 lbs test or not
14. Test 250 lbs: Boolean value based on whether the scale passed the 250 lbs test or not
15. Test 300 lbs: Boolean value based on whether the scale passed the 300 lbs test or not
16. Test 350 lbs: Boolean value based on whether the scale passed the 350 lbs test or not
17. Test 400 lbs: Boolean value based on whether the scale passed the 400 lbs test or not
18. Test 450 lbs: Boolean value based on whether the scale passed the 450 lbs test or not
19. Test 500 lbs: Boolean value based on whether the scale passed the 500 lbs test or not
20. Test 550 lbs: Boolean value based on whether the scale passed the 550 lbs test or not
21. Test 600 lbs: Boolean value based on whether the scale passed the 600 lbs test or not
22. Test Second 0 lbs: Boolean value based on whether the scale passed the second 0 lbs test or not
23. Negative Error Difference Total: Total amount of pounds underweighed by the scale throughout every test taken
24. Positive Error Difference Total: Total amount of pounds overweighed by the scale throughout every test taken
25. Fail Negative Error Difference Total: Total amount of pounds underweighed by the scale throughout every failed test
26. Fail Positive Error Difference Total: Total amount of pounds overweighed by the scale throughout every failed test


# Types of Results
1. Sealed: Passage of testing with any error found falling within allowable tolerance
2. Condemned: Failed test
3. Sealed Subject: Failed and most likely affecting the consumer positively
4. Not Sealed: Scale was not accessible at the time of inspection due to a multitude of reasons

# Methodology
I imported and analyzed the data, focusing on the amount of condemned scales compared to the total number of scales. I also analyzed data on John F. Kennedy International Airport and Laguardia Airport based on publicly available data on Open Data NYC. Based on my analysis, 2 scales were found to be inaccurate, with both found at JFK. This was out of roughly 500-600 scales. 
