# News-Sentiment-Analysis

### Overview

PapirMoney, a fictitious wealth management company, recently surveyed their customers and found that the customers were split into two distinct groups based on where they primarily get their financial news. One group read financial sites like Forbes and Fortune and the other group primarily read general news sites like the NY Times and ABC News.  

PapirMoney is getting ready to launch a marketing campaign and wants to know the overall sentiment towards the US economy as well as whether there is any difference in sentiment between the financial news and the general news sources.

With the results of this sentiment analysis, the marketing team will be able to adapt their strategy based on overall trends for the different potential customer groups.

### Data Sources

This analysis uses headlines and article descriptions from [News API](https://newsapi.org/).
The specific news sources included in the api call are:
 * ABC News
 * The Associated Press
 * Axios
 * Bloomberg
 * Business Insider
 * CBS News
 * CNN
 * Forbes
 * Fortune
 * Google News
 * Newsweek
 * The New York Times
 * USA Today
 * The Wall Street Journal

### NLP Model

The sentiment analysis was done using a HuggingFace pipeline API. The pipeline API uses a pre-trained NLP model, in this case the RoBERTa model, to classify the news articles. Since the intent of this analysis is to see the overall economic news sentiment of the two customer groups, a pre-trained model will give us those results with a much quicker turnaround. Writing an NLP and training it from scratch would be too time and labor intensive for this specific task.

### Results and Recommendations

The overall sentiment is trending slightly positive. The financial news sources show a reletively even sentiment over the past month, but the general news had several large swings.

In the world clouds, there are quite a few topics that appear in both the business and general articles. Mentions of AI, technology and innovation appear in the business cloud. Focusing the marketing strategy for this group on the innovations that PapirMoney is making would likely be well recieved. 

The words in the general news positive cloud focus more on jobs and consumers rather than technology. Inflation and housing also appear in the general news negative cloud. The marketing campaign for this audience should focus more on the security and stability that the product can provide, ratcher than the technical innovations.
