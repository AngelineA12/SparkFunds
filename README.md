# Investment Analysis for Spark Funds

## Problem Statement

Spark Funds is a venture capital firm looking to invest between 5 to 15 million USD in promising startups. The goal of this analysis is to help Spark Funds identify the most suitable investment opportunities by examining the following:

1. The most appropriate funding types that typically fall within the desired investment range.
2. The English-speaking countries that have historically received the most investments.
3. The main sectors that attract the highest investment amounts.

## Data Preparation and Cleaning

### Data Loading

We load the following datasets:
- **Companies Data**: Information about various companies, including the sector and country they belong to.
- **Rounds2 Data**: Details about the funding rounds, including the investment amounts and types.
- **Mapping Data**: Maps the numerous sub-sectors in the companies data to the main sectors.

### Filtering and Merging

1. **Investment Filtering**: We filter investments between 5 to 15 million USD.
2. **Country Filtering**: We include only countries where English is an official language.
3. **Data Merging**: We combine the companies and rounds2 data on the company identifier.

### Sector Mapping

We map each company's sub-sector to a main sector using the mapping file to standardize sector classifications.

## Analysis

### Investment Type Analysis

Objective: Identify the funding types (e.g., venture, seed, angel, private equity) that typically fall within the 5 to 15 million USD range.

Steps:
1. Calculate the average investment amount for each funding type.
2. Identify the investment types that match Spark Funds' preferred investment range.

### Country Analysis

Objective: Determine which English-speaking countries have received the most investments historically.

Steps:
1. Aggregate the total investment amount by country.
2. Rank countries based on the total investment received.

### Sector Analysis

Objective: Identify the main sectors that receive the most investment.

Steps:
1. Map each company's sub-sector to a main sector using the mapping file.
2. Aggregate the total investment amount by main sector.
3. Rank the sectors based on total investment received.

## Visualizations

1. **Investment Type Analysis**: A bar plot showing the average investment amount for each funding type within the desired range.
2. **Country Analysis**: A bar plot showing the total investment amounts by country.
3. **Sector Analysis**: A bar plot showing the total investment amounts by sector.

## Results

### Investment Type Analysis

The analysis identified several funding types within the desired investment range of 5 to 15 million USD. Notable among these are:
- **Venture**: Average investment of 8.91 million USD.
- **Private Equity**: Average investment of 9.23 million USD.
- **Debt Financing**: Average investment of 8.26 million USD.

### Country Analysis

The top English-speaking countries by total investment amount are:
1. **USA**: 122.40 billion USD
2. **GBR (United Kingdom)**: 6.56 billion USD
3. **CAN (Canada)**: 4.35 billion USD

### Sector Analysis

The main sectors receiving the most investment are:
1. **Others**: 23.55 billion USD
2. **Cleantech / Semiconductors**: 21.78 billion USD
3. **Health**: 7.16 billion USD

## Suggestions and Recommendations

### Investment Type Recommendation

Based on the analysis, **Venture** and **Private Equity** funding types are highly recommended as they fall well within the desired investment range and have substantial average investment amounts.

### Country Recommendation

The **USA** stands out as the most significant market for investments. It is recommended to focus on the USA, GBR (United Kingdom), and CAN (Canada) for high-potential investment opportunities due to their substantial historical investment amounts.

### Sector Recommendation

Investing in the **Cleantech / Semiconductors** and **Health** sectors is advisable, as they have received considerable funding historically, indicating strong market interest and potential for growth.
