---
title: "Dog-SEP - preregistration"
author: "Nina & Radek"
date: "03 April, 2020"
# csl: apa.csl
# bibliography: library.bib
output: 
  html_document: 
    highlight: pygments
    keep_md: yes
    number_sections: yes
    theme: united
    toc: yes
    toc_depth: 4
    toc_float: yes
editor_options: 
  chunk_output_type: console
---





# Study Information

## Title

Dog breeds as indicators of neighbourhood socioeconomic position.

## Authorship

Schnyder, N.^1^ & Panczak, R.^2^ 

^1^ Schuepfheim, Switzerland

^2^ Wloki, Poland

## Description/Background (detailed)

Australians love their dogs. Despite the fact that buying and owning one can add up to large expenses. 

Tracking socioeconomic position (SEP) of people and neighbourhoods is not a trivial task and usually requires access to comprehensive and high quality data that are often sensitive in nature. In the absence of individual-level SEP measures (such as income, wealth and education) area based measures are often used. Such measures usually use one statistical variable or use more to construct an index and use it to describe SEP of the area.

Census variables have been widely used for this purpose with more recent attempts leaning towards more exotic measures derived from night-time lights, mobile phones or car registrations to name few.

## Research Questions and Hypotheses

We will attempt to answer the question if the dog breed ownership data can be used as proxy for SEP of suburbs using the city of Brisbane, Australia as an example.

We assume that the cost of buying and maintaining the dog is a proxy for socioeconomic position of the owner. We hypothesize that the aggregated dog ownership data to the neighbourhhood level will closely reflect the traditional indices of SEP. 

---

# Design Plan

## Study Type

Observational study.

## Study design

Cross-sectional study.

## Blinding

No blinding is involved in this study.

## Randomisation

Not applicable.

---

# Sampling Plan

## Existing data

### Dog ownership

The `Dog ownership` dataset comes from the Brisbane City Council (BCC) [open data portal](https://www.data.brisbane.qld.gov.au/data/dataset/current-animal-related-permits/resource/c2823090-8a44-4c8b-9ed4-e988491b25f4). We will use `CARS - BIS - Open Data - Animal Permits Breed - 1 Jul 2019.csv` dataset that is closest in time to the `SEIFA` dataset. BBC's data portal does not provide earlier version of their data. Unfortunately, our attempts to contact BCC and obtain earlier version were not successful. In case the earlier dataset becomes available we will use that instead.

### Dog buying cost

To access data on `expensive dog breeds in Australia`, we typed these phrases into google. We selected the first two listings - [Australian Dog Lover](https://www.australiandoglover.com/2018/09/the-most-expensive-dog-breeds-in-2018.html) and [lifestyle](https://www.lifestyle.com.au/pets/most-expensive-dogs.aspx) - on google. The information of *Australian Dog Lover* was based on [Pet Insurance Australia](https://www.petinsuranceaustralia.com.au/the-most-expensive-dog-breeds/). We manually extracted the `Dog buying cost` data from *lifestyle* and *Pet Insurance Australia* on the 28 March 2020. Lifestyle provided information about prices of the top 20 most expensive dog breeds, Pet Insurance Australia did so for the top 10. 

### Dog insurance cost

We scraped the `Dog insurance cost` dataset from the Australian [Top 10 Pet Insurance](https://top10petinsurance.com.au/pet-insurance-prices/) website on the 30 March 2020. It provides insurance cost for the 0 most popular dog breeds in Australia. Insurance costs are based on a 1-year-old male, desexed dog with a 24-year-old owner living in Sydney (postcode 2010), Australia. The data lists the average cost of six Australian pet insurance providers separately for a comprehensive, an accident and an illness pet insurance with zero excess as of June 2017. 

### SEIFA

SEIFA indices are derived from 2016 census data and are available from the [Austrlian Bureau of Statistics](https://www.abs.gov.au/AUSSTATS/abs@.nsf/DetailsPage/2033.0.55.0012016?OpenDocument) (ABS).

We will search for associations of `Dog ownership` variables with all four indexes: 

  - The Index of Relative Socio-economic Disadvantage (IRSD); 
  - The Index of Relative Socio-economic Advantage and Disadvantage (IRSAD); 
  - The Index of Education and Occupation (IEO); 
  - The Index of Economic Resources (IER).
  
### Spatial data

We will use `State Suburbs ASGS Ed 2016 Digital Boundaries in ESRI Shapefile Format` from the [ABS](https://www.abs.gov.au/AUSSTATS/abs@.nsf/DetailsPage/1270.0.55.003July%202016?OpenDocument) as the primary definition of suburbs. Email correspondence from the BBC confirmed that these should match their data. Using this suburbs 

In case of inconsistencies, mismatches or name conflicts we will use `Locality boundaries - Queensland` data from the from Queensland Spatial Catalogue - [QSpatial](http://qldspatial.information.qld.gov.au/catalogue/custom/detail.page?fid={8F24D271-EE3B-491C-915C-E7DD617F95DC).

## Explanation of existing data and prior work based on this dataset

We explored frequencies of variables in `Dog ownership` data in order to resolve what analyses could be feasible. We checked the level of details in coding of the `Animal: Breed` variable. We also checked the values of the `Application Location: Suburb` variable in order to determine what spatial units were used for reporting and match that to the `SEIFA` data.

## Data collection procedures and brief description of data

All data has been collected and existed prior to the design of the study.

## Sample size and data inclusion/exclusion

Not applicable.

## Sample size rationale

Not applicable.

## Stopping rule

Not applicable.

---

# Variables

## Manipulated variables

Not applicable.

## Measured variables 

### Dog ownership

`Animal: Breed` variable. 

`Application Location: Suburb` variable. 

### Dog buying cost

We merged the two datasets informing on the buying cost of dog breeds (lifestyle and Pet Insurance Australia) into one dataset. Breeds that were named slightly different (e.g. typos, plural) but clearly referred to the same dog breed were treated as the same and corrected accordingly (e.g. Yorkshire Terrier and Yorkshire Terriers). This new dataset listed 20 expensive dog breeds and we named it "dog cost".

### Dog insurance cost

This dataset provides a variable on insurance cost for each breed compared to other breeds, which are categorised as "significantly above average", "above average", and "bellow average". 

## Indices 

Four `SEIFA` indicators come in the form of indices. As recommended by ABS, we will use deciles of indices.

---

# Analysis Plan

## Transformations

### Dog ownership

We combined the two datasets "dog cost" and "dog ownership" using the variables `breed` and `Animal: Breed`, respectively, storing information on names of dog breeds. We corrected for typos or plural to have a consistent set of dog breed names. Dog breeds that were listed both on the "dog cost" and the "dog ownership" dataset were considered to be expensive; dog breeds that were not listed on the "dog cost" but on the "dog ownership" dataset were considered to be not expensive; dog breeds that were listed on the "dog cost" but not on the "dog ownership" dataset were considered to be missing. We created a binary variable for dog buying cost (1=expensive, 0=not expensive).

The variable `Application Location: Suburb` will then be used to aggregate the expensive and total amount of dogs in the neighbourhood. These two variables will then be used to derive proportion.

### Dog insurance cost

As there are no guidelines on how to use the three categories "significantly above average", "above average", and "below average" of the `Dog insurance cost` dataset, we decided to collapse the categories in two different ways to receive two variables with two categories each.

First, we collapsed the categories "above average" and "below average". We created a binary variable for dog insurance cost (1=significantly above average, 0=not significantly above average). Second, we collapsed the categories "significantly above average" and "above average". We created a binary variable for dog insurance cost (1=above average, 0=bellow average).

## Missing Data

### Dog ownership

We will exclude cases with missing information on breed for all analyses. 

### Dog insurance cost

We will exclude cases with no link to information on the insurance cost in the analyses based on insurance data. 

### SEIFA

We will exclude neighbourhoods if one of the indices is missing for all analyses.

## Statistical methods and models, including sampling weights

### Means

We will calculate mean and SD values of percentage of expensive dogs per each decile of each SEIFA index. Expensive dogs will be define threefold - see definitions above in the ownership and insurance cost datasets.

### Correlations

We will divide neighbourhoods into deciles on the basis of percentage of expensive dogs among all dogs. Again, we will use three definitions of expensive dogs (see aboove). We will calculate Kendall’s correlation coefficient between these two deciles. We will also calculate agreement between two deciles by crosstabulating them and checking how many neighbourhoods agree on the decile (ie. are on the diagonal of the crosstabulation table).

### PCA index

Dog insurance data will be used to create share of all dogs in three categories in each neighbourhood: `Below average`, `Above average`, `Significantly above average`. These trhee variables will then be used to in PCA analysis and first component will then be sued to create continuous index. Index will be then divided into deciles and analysed in the same way as deciles of the proportions (see above). 

---

# Template info 

This preregistration document is been based on the [OSF Prereg](https://osf.io/zab38/wiki/home/) R Markdown template by James Bartlett [available here](https://github.com/BartlettJE/BartlettJE.github.io/blob/master/RMarkdown-scripts/OSF%20preregistration%20template.Rmd) incorporating parts of the template for secondary data preregistration by [Weston and colleagues](https://osf.io/x4gzt/), see also [here](https://osf.io/jqxfz/).

