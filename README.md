# optimal pricing strategy analysis
A data analysis project focused on understanding Uber's pricing, comparing competitors, and finding ways to improve revenue using Python, MySQL, and Power BI.

1. Business Problem -
What is the optimal pricing strategy for Uber to maximize revenue while maintaining customer demand and ride completion rates?

2. Dataset Overview - 
The analysis is based on the following dataset:
- 9,600 ride requests
- 8 Indian cities
- 5 ride categories: Auto, Bike, Mini, Sedan and Prime
- 3 ride-hailing platforms: Uber, Ola and Rapido
- November 2025 to March 2026

3. Project Workflow -
Step 1: Data Cleaning – Python
The first step was to prepare the raw datasets for analysis.
The following cleaning activities were performed:
- Removed duplicate records.
- Standardized platform, city and ride-type values.
- Converted date and numerical columns into the correct formats.
- Handled missing values 

Step 2: Data Analysis – MySQL
The analysis includes:
1) Revenue and average fare by ride type and platform.
2) Impact of surge levels on ride completion and revenue.
3) Revenue contribution from surged and non-surged rides.
4) Revenue and completion rates across different time slots.
5) Preliminary overall demand elasticity.
6) Preliminary demand elasticity by platform.
7) Platform comparison based on ride volume, completion rate, revenue, average fare and price per km.
8) Price per km comparison across ride types and platforms.
9) Promotional discount expenditure compared with completion rates.
10) Analysis of cancellation reasons by platform.
11) Relationship between surge pricing and completion rates within each ride type.
12) Uber promotional discount depth compared with completion rate, discount cost and revenue.
13) Uber's revenue contribution by time slot.
14) Comparison of Uber's ride-type mix against its revenue contribution.

Step 3: Business Intelligence – Power BI
An interactive Power BI dashboard was created to bring the analysis together.

4. Key Business Findings -

Finding 1: Uber has a premium pricing position
Uber generates ₹5,52,269 in completed-ride revenue, higher than Ola at ₹4,16,262 and Rapido at ₹1,66,163.
Its average fare is also higher at ₹201.26, while its ride completion rate stands at 73.06%, which is quite similar to its competitors.
Business implication: Based on the available data, Uber does not appear to need an overall price reduction. Its premium pricing position seems to be working reasonably well.

Finding 2: Prime and Sedan bring in a major share of revenue
Prime and Sedan together contribute around 50% of Uber's completed ride revenue, even though they account for only about 35% of completed rides.
Bike, on the other hand, contributes just 3.6% of total revenue lowest among all.
Business implication: Prime and Sedan offer better opportunities for revenue growth. Instead of focusing heavily on matching Bike prices with competitors, Uber could explore pricing improvements in these higher-revenue categories.

Finding 3: Surge pricing plays an important role in revenue
Around 91.5% of the combined revenue across all three platforms comes from surged rides. Still Uber's observed ride completion rate does not show a decline as surge levels increase.
Evening is Uber's strongest revenue-generating time slot, contributing 40.6% of revenue, followed by Morning at 26.3%.
Business implication: Surge pricing appears to be an important part of the revenue model. Continuing dynamic pricing while exploring additional opportunities during peak hours which could help improve revenue.

Finding 4: Higher promotional discounts do not always lead to better results
Uber's 10–20% promotional offers show higher completion rates than several of its deeper-discount offers.
For example, FIRST50 has a completion rate of 60.82%, compared with 73.03% for rides where no promotional offer was used.
Business implication: Offering bigger discounts does not necessarily mean more completed rides. A promotional discount cap of 20% could be tested to see whether Uber can reduce discount spending without affecting ride completion.

Finding 5: Price elasticity estimates
The preliminary estimates using fixed effects log-log are as follows:
Uber: -0.04
Ola: -0.04
Rapido: -0.35
These numbers reflect varying levels of price sensitivity between platforms, but are still preliminary and probably very rough.
Business implication: This information is not sufficient to make an assumption about inelasticity of prices for Uber users. Any fare change requires prior experimentation.

Finding 6: Cancellation rate is similar across platforms but varies by city
About 27% of ride requests on Uber platform do not materialize into ride bookings, which have a cancellation rate of 26.94%. This is almost identical to the figures for Ola (27.04%) and Rapido (26.61%).
In case of Uber, customer cancellations, driver cancellations and no driver found situations contribute to about 8-9% of total ride requests.
City-wise analysis reveals that the highest rate of cancellation belongs to Kolkata (29.74%) and Mumbai (28.28%). Meanwhile, Ahmedabad has the lowest rate of 23.52%, followed by Delhi (25.43%).
Business implication: In case of cancelled request, there is one missed revenue opportunity. The reason for high rate of cancellation can be explored further in case of Kolkata and Mumbai. However, each city has only about 460-490 requests on Uber platform.

Recommendations -
1) Maintain the present position regarding pricing - The average fare charged by Uber (₹201.26) is higher compared to those of the competitors, but their completion rates (73.06%) are more or less the same. There is no need for any pricing change according to the data obtained.

2) Focus on Prime and Sedan - Both these ride types account for 50% of revenue and 35% of completed rides. So pricing change is expected to have maximum impact here. Bike contributes only 3.6% of revenue, so matching other platform's prices on Bike appears to offer limited benefit.

3) Continue with surge pricing - In this case, the completion rates were found to remain steady as the surge level rises.

4) Promotional discount - Promotional discounts between 10% and 20% have generally performed better than larger discounts. the FIRST50 promotion achieved a completion rate of only 60.82%, while users who received no promotion had a higher completion rate of 73.03%. This indicates that offering larger discounts does not necessarily lead to more completed purchases or bookings. An upper limit on promotional discounts to maximum of 20% and focus on moderate discounts that encourage conversions without unnecessarily reducing revenue.

5) Testing and making changes - Elasticity values estimated in the analysis are preliminary. therefore, any changes in pricing, including a rise in prime fare or an upper limit for a discount, should be tested in small experiments and their effects should be measured.

6) Cancellations in cities - Uber has cancellation rates ranging from 23.52% in Ahmedabad to 29.74% in Kolkata. The cities with higher cancellation rates can be analyzed because each cancellation means a loss in revenue for the company.

7) Time slots - The two periods that generate the most income for Uber are evening (40.6%) and morning (26.3%), while the weakest is afternoon which may be an area for targeted offers.
