# Riftbound Unleashed - Personal Collection Analysis
## **Overview**
A data analysis project evaluating card rarity pull rates and distribution variance. Features a comparative Tableau dashboard analyzing personal hit rates against baseline box averages across multiple rarity tiers.
---
## Baseline Context

I opened 2 boxes, with each box containing 24 packs. Each pack is comprised of 14 cards.
To evaluate personal pull variance, the project references the official distribution matrix per pack and per box as established by the publisher (Riot Games). 

### Official Rarity Rates

| Rarity Tier | Pack Distribution | Box Average (24 Packs) |
| :--- | :--- | :--- |
| **Common** | 7 per pack | 168 per box |
| **Uncommon** | 3 per pack | 72 per box |
| **Rare** | ~2 per pack | ~41.6 per box |
| **Epic** | 1:4 packs | 6 per box |
| **Alternate Art** | 1:12 packs | 2 per box |
| **Overnumbered (ON)** | 1:36 packs | 0.66 per box *(~2 hits every 3 boxes)* |
| **Overnumbered Signature / Ultimate** | 1:360 packs | 0.06 per box *(~1 hit every 15 boxes)* |

> ***Note on Ultimate Rarity:** These baselines reflect the updated structural shifts introduced in the *Unleashed* set. The introduction of the Ultimate tier explicitly compresses the distribution margins of legacy sets like *Origins* and *Spiritforged*.
>> Verbatim from the Publisher: "Note that packs can only ever have up to one Ultimate Rare card, they will appear in < 0.1% of packs. Pack contents are randomized during manufacturing. Any stated appearance rates reflect averages across the print run and are not guarantees of appearance in booster packs or booster displays." (https://riftbound.leagueoflegends.com/en-us/news/announcements/the-unleashed-overview/)
---
## **Motivation**
I started this project to answer a simple curiosity: Did I actually beat the odds on my recent card pulls? 
To find out, I wanted to:
* Stop guessing with raw numbers: Seeing a total count doesn't tell me much. I wanted to see my actual hit percentages sitting right next to the official box averages so I could instantly spot the difference.
* Fix the scaling mess: It’s tough to map a massive __50%__ drop rate on the same screen as a tiny $0.6\%$ pull. Standard charts either cut off the highs or completely hide the lows.
* Make it easy to read: I wanted a clean, functional layout where I could glance at the data and immediately see exactly where I beat the curve and where I under-performed.
---
## Hypothesis
Going into this analysis, my baseline assumption was that my personal results would land **just below the official statistical average** in terms of pure yield. 

### Reasonings:
* **The "Feel" of the Pulls:** Based on comparisons of online videos where fellow players opened similar amounts of product, the raw frequency of high-tier hits felt slightly lower than commercial baseline expectations. 

---
## **Tools Used**
- Excel (Data Aggregation and Data Analysis)
- Tableau (Data Visualization)
---
## **Process**
* Counted and organized cards from my personal collection
* Organized by cards by rarity
* Aggregated and analyzed data within Excel
* Calculated average percentages based on publicly disclosed pull rates. (https://riftbound.leagueoflegends.com/en-us/news/announcements/collectability-in-riftbound-origins/)
* Calculated my personal percentages
* Connected Excel worksheet to Tableau
* Created visualizations of my analysis to communicate insights
---
## **Key Insights**
* When it came to the guaranteed portions of each pack, the numbers lined up perfectly e.g. Common, Uncommon, Inforamtional Inserts, and Tokens/Runes.
* Rares: difference of -0.44%.
* Epics: difference of -0.01%. (Likely my own rounding error)
* Showcases: difference of +.44%.
---
## **Dashboards**
<img width="856" height="1173" alt="image" src="https://github.com/user-attachments/assets/47902474-f330-487a-8f82-9317dff506aa" />
<img width="381" height="1170" alt="image" src="https://github.com/user-attachments/assets/7b36fb1c-3fd6-41de-90e6-530cc9fdb15a" />



---
## **Conclusion**
This project successfully shifted the analysis of card pull rates from raw guesswork to a structured, benchmark-driven model. 

### Key Takeaways:
* **The Verdict on Luck:** By comparing personal hit percentages directly against the baseline box averages, the data demonstrates exactly where variance swung in my favor (high-rolling specific top-tier slots) and where the distribution matched the expected average / guarantees.
* **Technical Success:** Replacing traditional, scale-limiting charts with a side-by-side horizontal asset layout solved the issues I had with visibility. It preserved the rare $0.6\%$ tiers while cleanly handling the massive $50\%$ baseline categories on a single, readable axis.

Ultimately, this dashboard proves that relying on raw data totals creates analytical bias. I underperformed in the Rare tier, but that was equally compensated (at least, percentage-wise) in the higher rarity tiers of Showcases. 

Moving forward, this framework can be easily scaled or unioned with additional volume data to track long-term distribution variance and/or variance normalization over time. 

---
## **Limitations**
* Sample Size: The data reflects a localized sample (672 total cards across 2 boxes). While this is no issue for personal analysis, it is relatively narrow compared to total commercial volume, meaning there is a certain degree of individual box variance.
* Data Limitations: Input data was recorded manually from live pull results, some margin of error from human data entry.
* Batch Variance: I sourced both of my Riftbound Unleashed boxes from the same retail store. However, there is no way for me to verify if the boxes originated from the same master case.
