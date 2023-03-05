# OSRS-Price-Predictions-for-Items-with-High-Trade-Volume
ECO481 ~ ML Project: Price Prediction for Runes in OSRS
# Current Status of the Project

This project is currently in its early stages, I have yet to implement the Random Forest method (nowcasting). For the time being, it includes the data collection code,
the merge csv file code, and the final csv dataset, that includes the prices over a (roughly) 90 hour period.

# Automated Rune Price Scraping.ipynb

Uses the api provided by the OSRS team to collect prices in 5 minute intervals, convert the information into dataframe objects, and then export as csv files.

# df_concat.ipynb

We convert the csv files (30 hours of price information each) into dataframes, concat them on the index, remove duplicates (same item name and timestamp) before exporting
it as a csv file.

# rune_prices_merged.csv

The final output, includes item name, timestamp, and average price over the 5 minute interval.
