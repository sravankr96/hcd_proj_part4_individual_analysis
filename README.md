[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)
![contributors](https://img.shields.io/github/contributors/sravankr96/hcd_proj_part4_individual_analysis.svg)
![codesize](https://img.shields.io/github/languages/code-size/sravankr96/hcd_proj_part4_individual_analysis.svg) 

# hcd_proj_part4_individual_analysis

This repository contains analysis of COVID impact on employment along with other policies like masking policies intended for the project part 4 for DATA 512 Human Centered Data Science course at the University of Washington - Masters in Data Science program

# Goal of this Project:

Over the past few years, the global pandemic has had an severe impact on all of us. This had a horrible, disruptive effect on many countries, and it greatly harmed the lives of countless people and their families.  One aspect of the pandemic's datafication that has been challenging to ignore during the past three years. In other words, a lot of data about the personal cost of the pandemic has been acquired, collated, and presented. With the aid of this information, we have the chance to look into the epidemic from a number of different perspectives in order to understand how it has impacted both individuals and society. 

In this analysis, the population of New Haven County is examined in relation to changes in job conditions as the disease develops through various stages of infection, fatalities and masked policy changes. Although it initially seems likely that unemployment would be at its highest during this epidemic, if we examine it closely, we can see that several industries had boomed in employment because of societal demands. A significant portion of the workforce was relocated to remote work in the interest of employee safety, however, as a result of the spread of the virus and rise in mortality. Given the numerous changes to immunization and masking laws, it makes sense that the employment trend has multiple peaks and dips. With the use of this analysis, we may approach these job shifts from a human-centric perspective and better comprehend how they affect the population's changing economic circumstances. In this analysis we primarily focus on the different aspects of employment – labor force, jobs availability, employed population, unemployed population as a whole and for individual employment sectors. With the help of statistical testing techniques, this analysis aims to validate the significance of COVIDs impact on different employment sectors.

We will be focusing on the analysis of one specific US county in this project - New Haven, CT, US.

## Datasource Information

1. RAW_us_confirmed_cases.csv: The RAW_us_confirmed_cases.csv file from the Kaggle repository of John Hopkins University COVID-19 data. This data is updated daily. You can use any revision of this dataset posted after October 1, 2022.
2. cdc_masking_mandates_county.csv: The CDC dataset of masking mandates by county. Note that the CDC stopped collecting this policy information in September 2021.
3. employment_*.csv: The U.S Bureau of labor statistics data containing labor force, jobs availability, employed and unemployed population details from 2018 to 2022.

## Repository Structure:
Here are the main folders in our github hcd_proj_part4_individual_analysis repository:
```bash
hcd_proj_part4_individual_analysis
.
├── LICENSE
├── README.md
├── data
│   ├── COVID-19_Vaccinations_in_the_United_States_County.csv
│   ├── CT_NewHaven_mask_mandate.csv
│   ├── RAW_us_confirmed_cases.csv
│   ├── education_and_health_services_employment_data-2018-2022.csv
│   ├── financial_activities_employment_data-2018-2022.csv
│   ├── government_employment_data-2018-2022.csv
│   ├── information_employment_data-2018-2022.csv
│   ├── laborforce_data-2018-2022.xlsx
│   ├── leisure_and_hospitality_employment_data-2018-2022.csv
│   ├── manufacturing_employment_data-2018-2022.csv
│   ├── mining_logging_construction_employment_data-2018-2022.csv
│   ├── nonfarm_employment_data-2018-2022.csv
│   ├── other_services_employment_data-2018-2022.csv
│   ├── professional_and_business_services_employment_data-2018-2022.csv
│   ├── raw_data
│   │   ├── education_and_health_services_employment_data-2018-2022.xlsx
│   │   ├── financial_activities_employment_data-2018-2022.xlsx
│   │   ├── government_employment_data-2018-2022.xlsx
│   │   ├── information_employment_data-2018-2022.xlsx
│   │   ├── leisure_and_hospitality_employment_data-2018-2022.xlsx
│   │   ├── manufacturing_employment_data-2018-2022.xlsx
│   │   ├── mining_logging_construction_employment_data-2018-2022.xlsx
│   │   ├── other_services_employment_data-2018-2022.xlsx
│   │   ├── professional_and_business_services_employment_data-2018-2022.xlsx
│   │   └── trade_transportation_utilities_employment_data-2018-2022.xlsx
│   └── trade_transportation_utilities_employment_data-2018-2022.csv
├── notebooks
│   └── hdc-512-part4-COVID_individual_analysis.ipynb
├── reports
│   ├── Part1_Reflection_Statement.pdf
│   ├── Part1_Visualization_Explanation.pdf
│   ├── Part2_Extension_Plan_Sravan.pdf
│   ├── Part3_COVID_impact_on_employment.pptx
│   └── Part4_Final_Report_Document.pdf
└── requirements.txt

```

We will follow a sequence of steps in this project

## 1. Dependencies and Setup

Python 3.10 is used to develop this project. Python package requirements are automatically installed when you execute the cells in the jupyter notebook.
Before proceeding with the execution of project in jupyter notebook, please replace the below line
```bash
  BASE_PATH = '/Users/sravan/PycharmProjects/DATA-512-HCD/hcd_proj_part4_individual_analysis'
```


## Missing data and Exception handling

It is possible that few of the dates does not have any mask mandating information in such cases we are assuming the mask mandating as 'No', meaning there is no masking policy in force at that point of time.

## Conclusion

In this analysis I intended to analyze the impact of COVID on the employment situation of New Haven County from multiple views of work force. The analysis is designed with human centric decision principles in consideration and aimed to produce a simple and explainable analysis to better understand the employment state. Different visual analysis techniques are applied to tailor the hypothesis for our analysis, which are then validated for significance using the statistical techniques Welch’s t test and Causal Impact Analysis. Though Welch’s test provided evidence to reject the null hypothesis, we utilized CIA to strengthen our evidence as the assumptions were weak in Welch’s t test.

## Authors
- [Sravan Hande](https://github.com/sravankr96)

![GitHub Contributors Image](https://contrib.rocks/image?repo=sravankr96/hcd_proj_part1_common_analysis)

## License
This work is licensed under MIT license. Read through the attached LICENSE file for more details about the use and distribution of this work.
# hcd_proj_part4_individual_analysis
