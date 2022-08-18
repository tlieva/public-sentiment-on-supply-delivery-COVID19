# Public Sentiment on the Supply and Delivery During COVID-19
Repository for machine learning research project compeleted for my postgraduate studies in Analytics for Business Decision-Making in MGMT 4084 - Digital Media Analysis.

## Project Background

#### Brief Introduction

The COVID-19 pandemic has brought about significant disruptions to the global supply chain that has led many companies to re-evaluate their strategies and the redesign of others under the new economic constraints (Meyer et al., 2021). The sudden shift of consumer spending behaviour had also left many global supply chains unprepared for the rapid change in consumer demand during the pandemic which saw an uptick in online shopping and local deliveries (Aryapadi et al., 2020). This further exacerbated the disruptions many supply chains and retailers faced and has exposed the vulnerabilities and critical points of the supply chain industry and identified the need to increase resilience to the supply chain industry worldwide (Meyer et al, 2021, Shih et al., 2020).

This research aims to analyze the implications of the ongoing COVID-19 pandemic on the supply chain industry. Using open-source Python to examine public sentiment and stock market performance of the industry during the pandemic, results of this research will serve as a basis for stakeholders to make more informed decisions to address deficiencies in the industry in anticipation of a fourth wave. Findings will also introduce new areas for future research in realizing the full impact of the pandemic on the industry post-pandemic. 

#### Research Objectives

This projects aims at; Examining Public Sentiments on Products Supply and Delivery During COVID-19 Pandemic and the Stock Market Reactions of the top five Supply Chain Firms during COVID-19 by identifying:

1. The most frequent words related to COVID-19 and product supply and delivery.

2. Public sentiments on product supply and delivery during COVID-19.

3. Stock market reactions for some of the top companies in the supply chain industry during the pandemic.



## Summary Methodology

#### Part 1: Examining Public Sentiment 
- Frequent keywords were identified by web scrapping comments from YouTube videos using open-source Python JupyterNotebook
- These videos were searched by querying the following keywords: ‘supply chain’, ‘delivery’,  ‘pandemic’, and ‘COVID-19’. 
- Only videos that had been uploaded in the last year were filtered for further sentiment analysis. This includes the period from which COVID-19 initially just started, up until October 2021. This ensures that content and public opinion will be relevant for the period during which pandemic was at its peak to highlight the public sentiment of the supply chain and delivery service during the pandemic. 
- Extracted data for each respective videos were subsequently exported to individual CSV files which were further compiled into one CSV file that was to be used for further sentiment analysis in python. 
- This generated results for the following: keywords in the form of a word cloud which identified the most **frequent words** associated with supply chain and delivery during COVID-19, **sentiment polarity**, and **sentiment subjectivity**.


#### Part 2: Stock Market
- Trend analysis was conduct on the adjusted stock market volume and price was conducted using Python, with subsequent outlier analysis completed on Excel.
- Data from March 1, 2020 to October 10, 2021 was extracted from Yahoo Finance online stock market platform, using Python Jupyter notebook. This platform provides a portfolio of free stock market data with access to real-time and historical data that had or are currently being traded in the market. 
- Selection of these companies were based on a 2021 Statista report on the top online stores worldwide in 2020, by e-commerce net sales, which found **Amazon, Walmart, Alibaba, Apple, and JD** to be some of the Top 10. **Alibaba**, was also selected due to its large presence in the Asian market and as one the biggest competitors to JD. 
- E-commerce net sales was the selected metric due increase in consumer online spending during the pandemic


## Summary of Findings & Recommendations
### Part 1: Public Sentiment
Results of polarity sentiment analysis regarding the supply chain and delivery service during the peak of the first and second wave appeared to be positive despite the significant disruptions faced by the industry in response to the unprecedented conditions brought by the COVID-19 pandemic (Figure 1).

**Figure 1. Polarity Sentiment Analysis**

<img width="512" alt="Screen Shot 2022-08-17 at 8 49 38 PM" src="https://user-images.githubusercontent.com/106416383/185268338-fc73aceb-e73d-46e0-bf4b-9e1500692a75.png">

Frequent keyword analysis shows words like shortage, manufacturing, government, need, supply, money, COVID, inventory, problem, shipping to be used in their statements, depicting the sense of worry for meeting demands and the unanticipated changes in the market due to regulations and safety compliances (**Figure 2**). More importantly, subjectivity analysis alone indicate that these sentiments among the consumer market are generally driven by personal opinions rather than on facts (**Figure 3**). 

**Figure 2. Frequent Keyword Word Cloud**

<img width="460" alt="Screen Shot 2022-08-17 at 8 51 37 PM" src="https://user-images.githubusercontent.com/106416383/185268540-b6aaf90f-1bbb-432c-abea-886547d98b6c.png">

**Figure 3. Subjectivity Sentiment Analysis**

<img width="489" alt="Screen Shot 2022-08-17 at 8 53 14 PM" src="https://user-images.githubusercontent.com/106416383/185268678-e8a7d83f-7caa-41dc-a86b-bf703b2f75f2.png">

Results of the examination of the overall public sentiment based on polarity and subjectivity scores of the public’s opinion in **Figure 4** highlights an overall neutral with a slight lean towards a positive perception held by the public on the state of the supply chain industry despite the challenges faced by many supply chain firms during the peak of the pandemic. This can be observed in the figure which presents a fairly even distribution of responses regarding the state of the supply chain and delivery service, suggesting that public sentiment is generally split.

**Figure 4. Polarity vs Subjectivity Scores**

<img width="479" alt="Screen Shot 2022-08-17 at 8 55 46 PM" src="https://user-images.githubusercontent.com/106416383/185268889-a1026cdc-e9f5-4697-8553-c12e4a24d325.png">

It is possible that people’s acceptance of the pandemic made them adjust to the new demands even though demands were not being fulfilled in totality.

### Part 2: Stock Market Reactions


# References
1. Meyer, A., Walter, W., & Seuring, S. (2021). The impact of the coronavirus pandemic on supply chains and their sustainability: A text mining approach. Frontiers in Sustainability, 2, 3. Retrieved from https://www.frontiersin.org/article/10.3389/frsus.2021.631182
2. Aryapadi, M., Chandra, V., Dekhne, A., Haddioui, K., Lange, T., & Venkataraman, K. (2020). Five actions retail supply chains can take to navigate the coronavirus pandemic. McKinsey and Company. Retrieved from https://www.mckinsey.com/industries/retail/our- insights/five-actions-retail-supply-chains-can-take-to-navigate-the-coronavirus-pandemic
3. Shih, W. C. (2020). Global supply chains in a post-pandemic world. Harvard Business Review, 98(5), 82-89. Retrieved from https://login.gbcprx01.georgebrown.ca/login?url=https: //search.ebscohost.com/login.aspx?direct=true&db=bth&AN=144910746&site=bsi- live&scope=site
4. Statista. (2021). Top online stores worldwide in 2020, by e-commerce net sales [report]. Retrieved from Statista.
