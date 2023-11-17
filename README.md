# Productivity-Score-Calculation
* This is the calculation of Productivity Score with min-max normalization for each item based on their Pcs Sold, First Cost, Gross Sales, and Contribution Margin on a SKU level, which will then be transferred back to item level. 
* This will then provide a rank to each item within each category and label "bottom 20%" items, which will serve as a guideline for discontinuation/liquidation of products.
   
*To understand the transformation and difference between item/stockey level and SKU level sales, refer to [Item-SKU-Forecast](https://github.com/raypan0625/Item-SKU-Forecast)*

## Terminologies
* Internally, most of the item level weeks on hand are simply calculated as total inventory divided by weekly sales. However, Amazon Innetwork/DI orders in batches (B2B) which might overstate our true sales speed. To smooth out our weekly sales numbers, we should calculate our true weekly demand.
   - **First_Date**: The first day of same month in the previous year
   - **Last_Date**: The last day of previous month in the same year\
   - **online_days**: How many days in a month a SKU is pushed online in a specific channel
   - **sku_hm_map**: The map created to streamline the process of transferring from SKU to HM and vice versa.
   - **C1**: Biggest catetory within the assortment, i.e. indoor, outdoor, parts, etc
   - **C32**: Smaller category dividing within C1, i.e. accent table, bar stool, dining chair, fire pit, etc.
   - **Pcs Sold**:
   - **First Cost**:
   - **Gross Sales**:
   - **Contribution Margin**:
   - **min-max normalization**
