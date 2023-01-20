# Public Sentiment on the Supply and Delivery During COVID-19
Repository for web scrapping research project. Completed for academic purposes.

## Project Background

#### Brief Introduction

The impact of the ongoing COVID-19 pandemic has exposed the vulnerabilities and critical points of the supply chain industry. The sudden shift of consumer demand has identified the need to increase resilience to the supply chain industry (Meyer et al., 2021; Shih, 2020). This was most evident in the manufacturing, procurement, and distribution of healthcare supplies in the early stages of the COVID-19 pandemic which led to delayed shipments and shortages of personal protective equipment (PPE) other essential medical supplies to the healthcare sector across the globe (Iyengar et al., 2020). Examples of these disruptions highlight the weak points of the current structure of the supply chain industry with many companies having implemented a lean supply strategy which focused on minimizing cost and maximizing efficiency through continuous reduction or elimination of waste (Shih, 2020; Swenseth & Olson, 2016). 

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


## Summary of Findings
### Part 1: Public Sentiment
Results of polarity sentiment analysis regarding the supply chain and delivery service during the peak of the first and second wave appeared to be positive despite the significant disruptions faced by the industry in response to the unprecedented conditions brought by the COVID-19 pandemic (Figure 1).

**Figure 1. Polarity Sentiment Analysis**

<img width="512" alt="Screen Shot 2022-08-17 at 8 49 38 PM" src="https://user-images.githubusercontent.com/106416383/185268338-fc73aceb-e73d-46e0-bf4b-9e1500692a75.png">

Frequent keyword analysis shows words like shortage, manufacturing, government, need, supply, money, COVID, inventory, problem, shipping to be used in their statements, depicting the sense of worry for meeting demands and the unanticipated changes in the market due to regulations and safety compliances (**Figure 2**). More importantly, subjectivity analysis alone indicate that these sentiments among the consumer market are generally driven by personal opinions rather than on facts (**Figure 3**). 

**Figure 2. Frequent Keyword Word Cloud**

<img width="460" alt="Screen Shot 2022-08-17 at 8 51 37 PM" src="https://user-images.githubusercontent.com/106416383/185268540-b6aaf90f-1bbb-432c-abea-886547d98b6c.png">

**Figure 3. Subjectivity Sentiment Analysis**

<img width="489" alt="Screen Shot 2022-08-17 at 8 53 14 PM" src="https://user-images.githubusercontent.com/106416383/185268678-e8a7d83f-7caa-41dc-a86b-bf703b2f75f2.png">

Results of the examination of the overall public sentiment based on polarity and subjectivity scores of the public’s opinion in **Figure 4** highlights an overall neutral with a slight lean towards a positive perception held by the public on the state of the supply chain industry despite the challenges faced by many supply chain firms during the peak of the pandemic. This can be observed in the figure which presents a fairly even distribution of responses regarding the state of the supply chain and delivery service, suggesting that public sentiment is generally split. It is possible that the public's acceptance on the stae of the ongoing pandemic has made consumers adjust to the new demands in the industry.

**Figure 4. Polarity vs Subjectivity Scores**

<img width="479" alt="Screen Shot 2022-08-17 at 8 55 46 PM" src="https://user-images.githubusercontent.com/106416383/185268889-a1026cdc-e9f5-4697-8553-c12e4a24d325.png">

### Part 2: Stock Market Reactions

_Stock Market Share Price_

Results of the trend analysis illustrates that the overall trend of the stock market performance in terms of market share price which saw Amazon’s performance consistently outcompeting its competitors throughout the period of the pandemic (Figure 5.) Note: Figure 6 shows the same data excluding Amazon due to significant difference in stock market performance. This is consistent with outlier analysis in Figure 7 which found, on average, the stock price of Amazon to outcompete its competitors.


**Figure 5. Stock Market Share Price** | **Figure 6. Stock Market Share Price (excl. Amazon)** 
---|--- 
<img width="589" alt="Screen Shot 2022-08-17 at 9 04 29 PM" src="https://user-images.githubusercontent.com/106416383/185269679-ed3804ca-286b-4f45-a6ac-3bd9eee98ca2.png"> | <img width="604" alt="Screen Shot 2022-08-17 at 9 04 40 PM" src="https://user-images.githubusercontent.com/106416383/185269693-a60eb129-9089-4a26-bfba-99fd5fc230b4.png"> 

When looking at both **Figure 5** and **Figure 6**, it can also be observed that an increase in stock market share price was observed by all companies during the start of the pandemic when COVID-19 was declared a global outbreak in March of 2020. This is to be expected as restrictions and social distancing measures that followed meant changes in consumer spending habits were inevitable and the pandemic saw an increase in online shopping and local deliveries which increased the market share value of some of the largest e-commerce companies in the supply chain industry. 

This trend remained consistent through the peak of the pandemic during the first and second waves and is most evidently demonstrated by Amazon in the outlier analysis shown in Figure 7 on the stock market price. 

**Figure 7. Stock Market Share Price Outlier Analysis**
<br>
_Outlier analysis of Amazon demonstrated extreme low values which occurred prior to the global outbreak, suggesting Amazon has been performing significantly better on average during the pandemic than usual prior to the pandemic._

<img width="532" alt="Screen Shot 2022-08-17 at 9 05 26 PM" src="https://user-images.githubusercontent.com/106416383/185269770-589bd60c-b9e9-4063-86eb-2127954b66cc.png">

As vaccines become available and countries begin to ramp up vaccination rates, we see the overall market share price to plateau. This is most evident in the months leading up to October 2021 and with many higher-income countries start to re-open, many brick-and-mortar businesses and social activities are to be expected to resume to some capacity (Charumilind et al., 2021). Despite this, the pandemic remains unpredictable and with the current dominant delta- variant of the coronavirus, this new wave of COVID-19 has put a pause to the transition of reopening in many countries even with high vaccination rates (Charumilind et al., 2021). Thus, it can be expected that stock market price of these companies to maintain its current performance but could increase with an impending third wave if countries begin pulling back on the plan towards reopening and demand increase.

_Stock Market Share Volume_

In terms of the stock market trading volume of these top supply chain firms, results of the analysis found volatility in the stock market throughout the pandemic (**Figure 8**). This is further supported by subsequent outlier analysis(**Figure 9**) which saw all five companies demonstrating abnormally higher trading volume than average since the start of the pandemic. This may be attributed to the uncertainty and unpredictability of the ongoing COVID-19 pandemic which has led to unprecedented disruptions to the global supply chain industry and increased pressure to sell stock. Moving forward, this trend is expected to remain unchanged in response to the uncertainty of the COVID-19 pandemic and the anticipation of an impending wave.

**Figure 8. Trend Analysis of Stock Market Share Volume**

<img width="640" alt="Screen Shot 2022-08-17 at 9 13 55 PM" src="https://user-images.githubusercontent.com/106416383/185270586-caf402d7-b3ae-4405-ae49-4e5b345d81ec.png">

**Figure 9. Stock Market Share Volume Outlier Analysis**

<img width="409" alt="Screen Shot 2022-08-17 at 9 14 59 PM" src="https://user-images.githubusercontent.com/106416383/185270685-a733d336-2247-4f6b-8ea8-19e6fb4a2efa.png">

## Conclusions
- Overall results of this study have identified a need for stakeholders to focus on developing a resilient supply network that can respond to unpredictable changes in the industry and consumer demand in anticipation of a fourth wave. 
- This will be necessary to improve the public sentiment on the current state of the industry and stock market performance based on findings of this research. Rise in stock market value of top firms in the supply industry coincided with periods of high trade volumes. 
- This Increased pressure to trade can be attributed to the lack of resilience and flexibility to respond to unprecedented conditions brought by the COVID-19 pandemic to meet consumer demand. 
- Significant delays and disruptions in the supply chain and delivery service had further downstream effects on the public's sentiment and has sparked discussions of the need for efficiency and digitalization of the supply network to meet consumer demand. 
- While there appeared to be a slightly more positive sentiment, the overall response was split. Firms will need to consider a more agile supply strategy and develop contingency plans that will offset disruptions and delays in response to unpredictable changes to the industry. 

_Recommendations_
- Need for diversifying the supply network to prevent dependency on a single supplier in which many companies lacked (Shih, 2020; Ferreira, 2021)
- Re-evaluate lean supply strategy which focused on minimizing cost and maximizing and consider a more flexible strategy 
- Moving the supply chains towards automation will also be the key to building a more resilient supply chain network

### Limitation

- In this research, the public sentiments on the supply chain and delivery service during the COVID-19 were analyzed based on data extracted from YouTube. This only represents a subset of population who use social media and have voiced their opinion regarding the industry and delivery service during the pandemic. Those who do not social media may not share the same opinion, which may bias the results of this research. 
- Similarly, majority of responses also represented the opinions of consumers who spoke English. The selected media used for this analysis was also published in English. This may also further misrepresent the opinion of members of the public who are not familiar with the language. 
- Future research will require gathering insights on the public sentiment through additional sources to ensure appropriate representation of the public sentiment on the impact of COVID-19 on the supply chain and delivery service.



# References
1. Meyer, A., Walter, W., & Seuring, S. (2021). The impact of the coronavirus pandemic on supply chains and their sustainability: A text mining approach. Frontiers in Sustainability, 2, 3. Retrieved from https://www.frontiersin.org/article/10.3389/frsus.2021.631182
2. Aryapadi, M., Chandra, V., Dekhne, A., Haddioui, K., Lange, T., & Venkataraman, K. (2020). Five actions retail supply chains can take to navigate the coronavirus pandemic. McKinsey and Company. Retrieved from https://www.mckinsey.com/industries/retail/our- insights/five-actions-retail-supply-chains-can-take-to-navigate-the-coronavirus-pandemic
3. Shih, W. C. (2020). Global supply chains in a post-pandemic world. Harvard Business Review, 98(5), 82-89. Retrieved from https://login.gbcprx01.georgebrown.ca/login?url=https: //search.ebscohost.com/login.aspx?direct=true&db=bth&AN=144910746&site=bsi- live&scope=site
4. Statista. (2021). Top online stores worldwide in 2020, by e-commerce net sales [report]. Retrieved from Statista.
5. Charumilind, S., Craven, M., Lamb, J., Sabow, A., Singhal, S. & Wilso, M. (2021). When will the COVID-19 pandemic end? McKinsey and Company. Retrieved from https://www.mckinsey.com/industries/healthcare-systems-and-services/our- insights/when-will-the-covid-19-pandemic-end
6. Ferreira, C. (2021). Disorders, vulnerabilities and resilience in the supply chain in pandemic times. MDPI AG. doi:10.3390/logistics5030048
7. Iyengar, K. P., Vaishya, R., Bahl, S., & Vaish, A. (2020). Impact of the coronavirus pandemic on the supply chain in healthcare. British Journal of Healthcare Management, 26(6), 1-4. doi:10.12968/bjhc.2020.0047 
8. Swenseth, S. R., & Olson, D. L. (2016). Trade-offs in lean vs. outsourced supply chains. International Journal of Production Research, 54(13), 4065-4080. Retrieved from https://login.gbcprx01.georgebrown.ca/login?url=https://search.ebscohost.com/login.aspx?direct=true&db=bth&AN=118193646&site=bsi-live&scope=site
