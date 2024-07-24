# ml-capstone

## Word Embeddings and LLMs on 10K and 10Q Filings

### ABSTRACT

The 10-K and 10-Q filings submitted to the SEC by all publicly traded U.S. companies have a huge amount of information. Many valuable insights can be drawn from these filings. However, due to the size of the filings and the comprehensive nature of these filings, it is very hard to draw insightful conclusions. In this paper, we aim to construct a vector database that stores textual information in numerical form. This numerical vector for every firm is calculated using various Natural Language Processing (NLP) techniques. This paper also aims to find companies that are the most similar to each other which can give businesses valuable insights into investment strategies. The other topics that this paper touches upon include classifying companies based on the GICS code and identifying profit pools within industries. The report successfully demonstrates the utility of NLP in financial analysis, offering new perspectives for strategic investment and company assessment.

The project is designed to accomplish the following objectives -
• Vector Database Construction: The first step is to construct a robust and comprehensive vector database that incorporates both key financial indicators and textual content from SEC filings. Specifically, the database will focus on sections of the 10-K and 10-Q filings like Risk Factors, Management’s Discussion and Analysis (MD&A), and Business Descriptions. This vector database will serve as the first step towards building more complicated language learning models which can then be used to assess companies across various industries.
• Similarity Search Language Model: The second step is the utilization of NLP techniques to create a sophisticated language model capable of analyzing the vast textual content found in SEC filings. The model will quantify sentiment and assess how different companies relate to one another, es- pecially within supply chains. By identifying such correlations, the project aims to offer deeper insights that could be crucial for investment strategies and risk assessment. To find the companies that are similar to each other we closely follow the cosine similarity methods highlighted in [1].
• GICS & Company Profit Pools: Another objective of this research project is to employ NLP algo- rithms to identify notably profitable companies within specific industries in the U.S. market. The aim is to go beyond mere profitability metrics to understand each company’s role and leadership within broader industry trends and competitive landscapes. This will be achieved by scrutinizing targeted sections of SEC filings that focus on profitability, market share, and competitive position- ing. The insights gained will serve to guide investment strategies and business decisions.


### FINDINGS

This project successfully demonstrated the efficacy of various analytical methods in assessing company similarities and GICS classification, using advanced techniques like SVD, TF-IDF, and various machine learning models. The results highlighted the significant impact of word co-occurrence and contextual relevance in determining company similarities, with the co-occurrence matrix combined with SVD yield- ing particularly insightful outcomes. For the GICS classification, the superiority of ensemble methods like XGBoost was evident, showcasing their robustness and accuracy in handling complex datasets. The profit pools analysis further enriched our understanding, revealing both well-known and lesser-known companies as significant contributors to industry profits, emphasizing the importance of in-depth finan- cial analysis. The flexibility and adaptability of the developed tools pave the way for broader applications, potentially encompassing a wider array of companies and financial metrics.

For future scope, this project opens up several avenues for further research and development. One po- tential area of expansion is the application of these methods to a larger dataset, extending beyond the S&P 500 companies to include more firms from Russell 3000 and even international corporations, which would provide a more comprehensive view of the global market dynamics. Additionally, integrating real- time data analytics could offer more up-to-date insights, crucial for investment and strategic business decisions. The incorporation of AI and machine learning algorithms for predictive analysis can also be explored to forecast market trends and company performances. Furthermore, we could use other kinds of pre-trained word embeddings like FinBert and see whether the accuracy can be increased. Overall, the project sets a solid groundwork for future explorations, offering significant potential for enhancing and broadening the scope of financial analysis and insights.

### REFERENCES

[1] Vamvourellis, Dimitrios, et al. ”Company Similarity using Large Language Models.” arXiv preprint arXiv:2308.08031, 2023

[2] https://simonwillison.net/2023/Aug/27/wordcamp-llms/retrieval-augmented-generation 

[3] https://sec-api.io/docs/sec-filings-item-extraction-api/python-example



