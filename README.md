# **India's Healthcare Infrastructure Analysis**

## OVERVIEW: 
This project analyzes the healthcare infrastructure across Indian states using government-published data from Rural Health Statistics 2021-22. It presents insights on the availability and adequacy of Primary Health Centres (PHCs), Community Health Centres (CHCs) and Sub-Centres (SCs) in relation to population needs. By analyzing healthcare facility distribution relative to population, the power-bi dashboard helps users in exploring underserved states where health infrastructure is lacking.

## PROBLEM OBJECTIVE: 
India has one of the largest populations in the world, but does everyone have equal access to basic healthcare? With millions depending on government facilities like Sub Centres (SCs), Primary Health Centres (PHCs), and Community Health Centres (CHCs), it's important to ask:
  * Is healthcare infrastructure evenly distributed across states?
  * Which states have adequate public health coverage and which fall short?
  * How many facilities are required, and how many actually exist?
  * Are both urban and rural populations adequately served, or are there noticeable gaps?

This project aims to uncover which states are well-equipped, which are lagging, and how large the shortfall is, by comparing population needs with available infrastructure. using real government data.

## DATASET USED:
 *  Rural Health Statistics 2021–22
 *  Source: Ministry of Health and Family Welfare, Government of India
 *  Includes data on required, existing, and shortfall numbers for SCs, PHCs, and CHCs (covers both rural and urban areas). Also provides state-wise projected population (rural & urban), used to calculate population to type of facility ratios.
 * Format: PDF: cleaned and organized using **Excel**

### Excel Cleaning:
I used Excel to extract and clean the data tables from the Rural Health Statistics PDF. This included removing totals, notes, special symbols, and any rows that didn’t contain actual data. I also fixed state names to make sure they were consistent across all sheets.

### Power-Bi:
 * Imported the cleaned data on healthcare facilities, population, and shortfall into Power BI.
 * Built a data model by establishing relationships between the tables using the state column as the common key.
 * Created DAX measures to calculate key metrics like the total number of facilities, average population served per facility, and the share of rural population.
 * Designed additional DAX-based tables to show facility distribution by type (SC, PHC, CHC) and area (rural/urban), along with people served per facility.
 * Added interactive slicers for state selection and population tier, allowing users to filter and compare regions easily.
 * Designed navigation buttons to move between the Overview and individual pages for SCs, PHCs, and CHCs, making the dashboard more comprehensive.

### Dashboard Pages
1. Overview
* Shows total number of health facilities (SCs, PHCs, CHCs) across India, categorized by rural and urban area type.
* KPI cards like how many people are served by each facility on average, rural population etc.
* Bar charts compare top states by population and available health centres.
* Quick view of where shortfalls in infrastructure, whether PHCs, CHCs or sub-centres are the highest.
* Population comparison between urban and rural areas.

2. PHC Page (Primary Health Centres)
* Shows how many PHCs are required vs how many exist state-wise.
* Urban vs rural PHC numbers.
* States with the largest shortfall in PHCs.
* PHC access compared to population reveals major gaps.

3. CHC Page (Community Health Centres)
* Focus on secondary care centres.
* Shows which states have fewer CHCs than needed.
* Includes rural vs urban distribution.
* CHC access compared to population reveals major service gaps.

4. SC Page (Sub Centres)
* Shows total number of SCs and compares to required numbers.
* Highlights how basic healthcare is spread across rural and urban areas.
* States with large gaps in coverage (e.g., UP, Bihar) clearly visible.
  
## Insights
* Rural–urban imbalance can be clearly seen: While 65.15% of India’s population is rural, healthcare facilities are not proportionately distributed, leaving rural areas under-served across all levels—Sub-Centres, PHCs, and CHCs.
* Sub-Centres are the most widespread accounting for almost 162k, but still fall short in high-population states. Uttar Pradesh and Bihar alone account for a shortfall of over 27K Sub-Centres.
* PHC access is also highly inadequate:
   * Only 45% of the population is adequately covered.
   * 111 million people (8%) face critical gaps in PHC access.
   * Top shortfall states include Uttar Pradesh, Bihar, and West Bengal.
* It can be noticed that CHCs are the most strained facility type:
   * One CHC serves over 227,000 people on average, far above recommended norms i.e around 120,000
   * Only 26% of the population is adequately covered, showing extreme gaps.
   * 176 million people (12.7%) face critical coverage gaps.
* States like Uttar Pradesh, Bihar, Maharashtra, and Madhya Pradesh consistently appear among the worst-performing in terms of shortfall across all facility types.

## Conclusion
* The data highlights a major gap between rural healthcare needs and available infrastructure. Although over 65% of India’s population lives in rural areas, the number of Sub-Centres, PHCs, and CHCs falls far short, especially in large states like UP, Maharashta etc. These gaps directly affect millions of people who struggle to access basic health services.
* This issue is even more serious considering that these shortfalls existed during the COVID-19 pandemic. At a time when strong healthcare systems were crucial, many rural areas remained unprepared. Such gaps during a crisis can be or most likely were devastating for already vulnerable populations.
* To close these gaps, India must invest in expanding and upgrading rural health infrastructure, ensuring facilities are not only built but properly staffed and equipped. This is essential for both everyday care and future health emergencies.


