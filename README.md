# Wine Glass, Flight & Tasting Sales: Year-to-Date Comparison Across Locations
🍇 Unionville Vineyards (Ringoes, NJ)

<img width="1040" height="675" alt="image" src="https://github.com/user-attachments/assets/afa47e8c-5633-4bbf-aeee-0385b7235e07" />

---
## About Unionville Vineyards 
Unionville Vineyards is a premier boutique estate winery nestled in the pastoral hills of Hunterdon County, New Jersey. Spanning over 80–90 acres of preserved farmland, Unionville manages multiple estate vineyards — Home, Amwell Ridge, Pheasant Hill, and more — each chosen to express the unique terroir of central and northern NJ.

The team practices minimal‑intervention viticulture and winemaking, emphasizing sustainable farming and letting the vineyard speak for itself. Their winemaking honors an old‑world tradition, avoiding over‑oaking to preserve the wine’s natural acidity, fruit expression, and transparency.

Unionville is widely considered the best winery in New Jersey, consistently producing fruit‑forward, aromatic wines. Their commitment to terroir-driven wines set a gold standard in NJ winemaking.

---

## About the Project

Retained by Unionville to design and deliver sales reports for 3 specific sales categories.

Objective: How many glasses of wine, wine flights, and wine tastings were sold YTD across two locations, Ferry Market Wine Bar (New Hope, PA) and Unionville Tasting Room (Ringoes, NJ) in comparison to the same date range in 2024, 2023, 2022, and 2021?

Solution: Create a custom ETL script to merge, clean, and structure historical sales data from Shopify and POS systems.

  - The process began by extracting the full sales history from Unionville's e-commerce platform of choice, Shopify. All winery sales, ranging from online wine purchases to on-premise sales of cheese boards, sandwiches, and wine bottles purchased through their POS system ultimately transact through Shopify.
  - Loaded sales history across multiple CSV files and concatenated into a single dataset (DataFrame) to begin the data wrangling process using Pandas, an open-source data analysis and manipulation library built on top of NumPy.
  - Data wrangling techniques included filtering, grouping, and use of .ffill() and .bfill() methods across various columns within the sales orders. For example, various sales orders' columnar data, including `Location`, `Tax 1 Name`, and `Paid At` were intermittently missing or otherwise did not export.
  - Time series analysis requiring parsing separate datetime string formats and transforming into a single consistent datetime format for proper filtering, grouping, and joining.
