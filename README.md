Cocoa Cooperative — Farmer Yield Analysis (2025/26 Season)
Author: Cecil Nii Ayikai Tetteh  
Tools: Microsoft Excel  
Domain: Agricultural Data Analytics · Cooperative Management · Ghana Cocoa
---
## Project Overview
This project analyses farmer-level cocoa delivery and yield performance for a cocoa cooperative in Ghana during the 2025/26 main crop season.
The cooperative supplies cocoa to an international premium chocolate buyer under a fixed offtake agreement. The analysis was built to help cooperative management move beyond raw delivery totals and understand which farmers and communities are performing well, which are underperforming, and what the cooperative's true production capacity looks like.
---
## Problem Statement
The cooperative holds biodata and spatial (GPS/geodata) records for 2,382 registered farmer members across 26 communities. Each season, delivery records are captured per community in separate spreadsheets.
The core questions this project answers:
What is each farmer's yield efficiency — kilograms of cocoa per hectare of farm?
Which communities are the highest and lowest performers?
How many registered members actually delivered this season, and what does the gap tell us?
How does the cooperative's total supply capacity compare to the client's offtake requirement?
---
## Data Sources
Dataset	Description
Farmer delivery records	Season totals per farmer across 26 community sheets
Cooperative spatial master	GPS-surveyed farm boundaries with measured plot areas (hectares)
Both datasets were anonymised for this portfolio. Farmer codes follow the cooperative's internal ID structure (e.g. `KCO/Z02/ABE/002`).
---
## Methodology
Step 1 — Data consolidation  
26 individual community delivery sheets were merged into a single flat table of 681 farmer records.
Step 2 — Area matching  
Each farmer's delivery record was matched to their measured farm area from the spatial master using their unique farmer code. Where a farmer holds multiple plots, areas were summed to give total farm area.
Step 3 — Yield calculation  
Yield per hectare was calculated as:
```
Yield (Kg/Ha) = Total Delivery (Kg) ÷ Total Farm Area (Ha)
```
Step 4 — Performance tiering  
Farmers were classified into three tiers based on yield:
Tier	Threshold
High	≥ 400 Kg/Ha
Medium	200–399 Kg/Ha
Low	< 200 Kg/Ha
Step 5 — Community summary  
Individual farmer results were aggregated to community level to identify spatial patterns in yield performance.
---
## Key Findings
Delivery participation
681 of 2,382 registered farmers (28.6%) made deliveries this season
The 1,701 non-delivering members represent significant untapped supply capacity
Possible reasons include side-selling to local traders, inactive farms, or poor mobilisation
Season volume vs. client requirement
The client's offtake requirement: 750 MT
Actual cooperative delivery this season: ~749.8 MT
The cooperative met its target almost exactly — but with less than a third of its membership
Yield performance
Cooperative average yield: 637.5 Kg/Ha
Highest-performing community: Boakyekrom — 769.7 Kg/Ha
Lowest-performing community: Sunkwa — 477.4 Kg/Ha
The gap between best and worst community is ~60%, suggesting significant variation in farm management, input use, or tree age across zones
Supply capacity estimate
If all 2,382 registered farmers delivered at the current average yield and average farm size, estimated total supply would exceed 1,700 MT — more than double the current client requirement. This positions the cooperative to pursue additional offtake agreements with other premium buyers.
---
## Recommendations
Investigate non-delivering farmers — differentiate between side-sellers, inactive farms, and mobilisation failures. Each requires a different intervention.
Target extension services at low-yield communities — Sunkwa, K. Kuma, and Tano Odumase show the most room for improvement.
Use yield data for input planning — high-area, low-yield farmers are the highest-leverage targets for fertiliser or agrochemical support.
Explore additional offtake agreements — the cooperative's data infrastructure (spatial records, farmer codes, yield history) is a competitive asset when approaching new buyers.
---
## Files
File	Description
`Delivery_Yield_Analysis.xlsx`	Main analysis workbook — Community Summary dashboard + full farmer detail
---
## About the Author
Cecil Nii Ayikai Tetteh is a GIS and Data professional based in Ghana with experience in agricultural data management, spatial analysis, and cooperative operations. He holds a BSc in Natural Resources Management from KNUST and certifications in Data Analytics from ALX Africa.
LinkedIn · GitHub
