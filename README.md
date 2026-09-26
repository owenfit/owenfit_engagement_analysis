# OwenFit Engagement Analysis

I analyzed 172 Instagram Reels from my OwenFit account to understand which content types receive the most views and how engagement metrics relate to views.

## Interactive Dashboard

[View the OwenFit Tableau dashboard](https://public.tableau.com/views/Book1_17615359491380/OwenFitOverview?:language=en-US&publish=yes&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Questions

* Which content types have the highest median and average views?
* Which engagement metrics are most strongly associated with views?

## Data and Tools

The dataset contains reels posted from March through August 2026. I recorded the metrics in Excel and analyzed them using Python, pandas, NumPy, and Matplotlib in Google Colab.

Each row represents one reel, with its content type, views, video length, and engagement metrics.

I also used Tableau Public to build a dashboard comparing views across content types and showing how nine engagement and retention metrics relate to views.

## Methods

* Checked for missing values, duplicate post IDs, and invalid numeric values.
* Compared mean and median views across nine content types.
* Calculated Spearman correlations between views and nine metrics: skip rate, length, share rate, save rate, like rate, repost rate, comment rate, percent watched, and average watch time.
* Created charts to compare content performance and metric associations.

## Main Findings

* Talking videos had the highest mean views: 149,960 across nine reels. Their median was 4,907, showing how strongly viral posts influenced the average.
* Skip rate had the strongest negative association with views, with a Spearman correlation of approximately −0.56.
* Average watch time had the strongest positive association, at approximately +0.56.
* Share rate (+0.48), percent watched (+0.46), and repost rate (+0.43) also had positive associations with views.
* Video length (+0.03) and comment rate (−0.04) showed little association with views.

## Limitations

This analysis covers one account, and the content categories have uneven sample sizes. Other and Transformation contain only two reels each. Posts also had different amounts of time to accumulate views.

Accounts Reached was excluded because some reported values appeared unreliable. For 18 reels, I used Instagram’s reported engagement rates instead of calculating them from the questionable reach values.

## Files

* `OwenFit_Engagement_Analysis.ipynb`: Code, charts, and written interpretations.
* `OwenFit Engagement Data-2.xlsx`: Source dataset.

## How to Run

1. Download the notebook and Excel dataset.
2. Open the notebook in Google Colab.
3. Run the first cell and upload the Excel dataset when prompted.
4. Run the remaining cells in order.

