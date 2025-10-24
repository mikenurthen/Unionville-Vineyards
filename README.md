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

Solution: Create an automated ETL script to merge, clean, and structure historical sales data.
  - The process began by extracting all historic sales data from Unionville's e-commerce platform Shopify. Both on-premise retail POS sales and online DTC sales transact through Shopify.
  - Time series analysis requiring parsing separate datetime string formats and transforming into a single consistent datetime format for proper filtering, grouping, and joining.


### Recent Improvements

<b>Refactored for Modularity and Automation</b>
<b>Modularized Codebase:</b> Wrapped major processing steps (data cleaning, parsing, and visualization) into well-defined functions for better readability, testing, and reusability.

<b>Automated File Watcher:</b> Implemented a continuous monitoring loop that automatically detects, loads, and integrates new CSV files into the master dataset without manual intervention.

<b>Batch Processing Logic:</b> The watcher now processes all newly detected files together before triggering downstream analysis and visualizations, ensuring consistency and performance.

<b>Improved Error Handling:</b> Added validation for column types and data integrity checks to catch and report problematic rows in real time.

<b>Scalable Data Pipeline:</b> Designed the workflow to handle incremental data ingestion, enabling scalable ETL-style data updates and analytics.
