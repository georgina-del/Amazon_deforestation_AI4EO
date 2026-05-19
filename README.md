# Detecting Deforestation in the Amazon Regions of Para and Rondonia Using K-means Unsupervised Learning 

## Table of contents

## Project Overview

## Background and Motivation 

The Amazon rainforest is one of the most crucial biomes on the planet, often called the “lungs of the Earth” due to its ability to regulate Earth’s climate. The Amazon is a colossal 6.7 million square kilometres stretching across nine South American countries and is host to over 30,000 plants, it is the most diverse ecosystem on Earth (Ferreira, 2026). In addition to this, the Amazon is the biggest land sink of Carbon and is estimated to store 140 billion tonnes of carbon (Greenpeace, 2020). However, since the 1970s rapid land-use change has meant that deforestation has been occurring at accelerating rates in order to meet population demand, in 2019 alone there was a 34 % increase in forest clearing from the previous year (Santos et al., 2024 , Teixeira et al., 2025). Without proper policy it is estimated that deforestation could reach up to 50% of the 2050 (Borma, Nobre and Cardoso, 2013).  

Deforestation has huge consequences on the Amazon rainforest and the Earth system as a whole. Recent studies suggest that deforestation, forest damage, and climate change have caused parts of Southeastern Amazonia to shift from absorbing carbon dioxide from the atmosphere to releasing more carbon than they store, amplifying initial perturbations (Teixeira et al., 2025). The lower number of trees reduces atmospheric moisture, altering precipitation patterns across the Amazon region by causing longer dry seasons and more frequent droughts (Borma, Nobre and Cardoso, 2013). This increases the Amazon’s vulnerability to wildfires, which further destroy ecosystems and threaten biodiversity (Borma, Nobre and Cardoso, 2013). 

Given the scale and urgency of Amazon deforestation, effective monitoring is essential for informing conservation policy. Knowing the rate, location and type of forest loss is therefore the first and most fundamental step toward slowing it and hold high-deforestation regions accountable. Traditional ground-based surveys are logistically challenging, expensive, and unable to provide the spatial coverage needed to track deforestation across millions of square kilometres. Satellite remote sensing offers a powerful alternative,repeatable, and low-cost monitoring of land cover change at regional scale. This project leverages freely available Sentinel-2 multispectral imagery accessed via Google Earth Engine to apply K-means unsupervised machine learning to detect and quantify forest loss.

## Data Acquisition and Study Area

The dataset used in this study consists of Sentinel-2 Level-2A surface reflectance imagery, accessed via Google Earth Engine (GEE) through the ESA Copernicus programme. Sentinel-2 was selected for its 10 m spatial resolution, 5-day revisit time, and 13 spectral bands covering visible, near-infrared and shortwave infrared wavelengths, making it well suited for vegetation analysis and land cover change detection at landscape scale (CDSE, 2023).

The notebook automatically selects the least cloudy available image for each region and year by searching the full calendar year and ranking by cloud cover percentage. Manual override functionality is also included to allow selection by index where the automatic choice had unfavourable cloud conditions over the specific study area. This was necessary for the Pará region where the default images were heavily masked, requiring dry season images to be selected manually.

Brazil was selected as the study country as it contains the largest area of tropical rainforest in the world and has the highest absolute rates of deforestation globally, making it one of the largest national emitters of greenhouse gases from land use change (Santos et al., 2024; Ferreira, 2026).

**Sentinel-2 Satellite Images of Cacoal, Rondônia, Brazil**

**Location:** Central Rondônia deforestation hotspot

**Coordinates:** 11.45° S, 61.1° W

**Bounding box:** [-61.3, -11.6, -60.9, -11.3]

**Characteristics:** Rondônia is located in Western Brazil, it is characterised by the distinctive fishbone deforestation pattern where agricultural clearings branch off road networks into intact forest and records among the highest deforestation rates in Brazil (Ferraz, Vettorazzi and Theobald, 2009)

**Image 1 (Baseline):** 2020 dry season

**Image 2 (Recent):** 2024 dry season


**Sentinel-2 Satellite Images of Altamira, Pará, Brazil**

**Location:** Altamira municipality, southern Pará

**Coordinates:** 3.65° S, 52.2° W

**Bounding box:** [-52.4, -3.8, -52.0, -3.5]

**Characteristics:** Pará is the second largest state in Brazil and is consistently identified as one of the most deforested municipalities in the entire Amazon basin (Ferraz, Vettorazzi and Theobald, 2009). The region sits on an active agricultural frontier where primary forest is being converted to cattle pasture and smallholder agriculture at high rates. 

**Image 1 (Baseline):** 2020 dry season

**Image 2 (Recent):** 2024 dry season


## Methodology 


## Results and Performance

## Key Findings


## Environment Impact Assesment 


## Limitations and Future Work 
