# **Content-Based Article Recommender System**
Section and Team Number : B1 Group 12
Members :Divyam Rana, Rinaldo Patel, Siddharth Kant, Yash Kothari

# **About our Project**
The exponential growth of digital content has made it increasingly difficult for users to discover relevant articles tailored to their interests. Our project aims to develop a content-based recommendation system that clusters and suggests relevant articles without relying on predefined labels. This system will enhance user engagement by providing personalized reading recommendations, ensuring that high-quality content reaches the right audience, and increasing retention rates on news platforms.

# **Business Relevance:**
Traditional recommendation systems, based on simple keywords or broad demographic data end up missing the mark to grasp what the readers actually care about, which leads to lower  engagement rate, high bounce rates and major revenue loss from ads. For CNNs Daily Mail thousands of articles published everyday, it's easy for great content to be buried. That’s where our project comes in. Our AI-driven system will enhance:
- Improve **user engagement** by delivering personalized recommendations leading to longer session durations, lower bounce rates, and increased content consumption.
- Help publishers **identify emerging trends** and repurpose relevant articles.
- **Increase ad revenue** through targeted content delivery, improving ROI for advertisers and boosting programmatic ad revenue.
- **Scale efficiently** to handle vast amounts of news data in real time and allowing them to focus on higher-value editorial strategies.
  
**Real-World Applications**: The insights from our project have multiple business applications:
**News Media:** Personalized article recommendations to increase user dwell time.
E-Commerce & Marketing: Content recommendations based on user interest.
Academic Research: Automated categorization of research papers for better discoverability.

# **Supporting Industry Context & Sources:**
- Smith, J. (2023). "Personalization in Digital Media: The Future of Engagement." Journal of Digital Trends.
- Thompson, R. (2022). "AI-driven News Recommendation Systems." Media Analytics Review.

#**Problem Statement**
In today’s fast paced, reel-scrolling digital world, keeping readers engaged is a major challenge for media companies. People are constantly bombarded with news, and if they don’t find content that truly interests them, they quickly lose interest and move on. The main objective of our project is to create an intelligent recommendation system for news articles that enhances content discoverability without requiring manual categorization. Our specific objectives include:
- Identifying patterns in large-scale unstructured text data.
- Implementing NLP techniques to extract meaningful insights.
- Applying unsupervised learning methods such as topic modeling and document similarity heuristics.
- Developing a content-based recommender system to improve user engagement.
This system will enhance user engagement, improve content discovery, and provide a seamless reading experience by reducing the effort required to find relevant articles. The recommender will be designed for news platforms, academic journals, or online media, ensuring that users receive high-quality, contextually relevant content suggestions.

#**Findings and Interpretations**

The following are the final findings and interpretations for our project. These are based on what we found in the analysis and experimentation section coupled with the exploration of data.
EDA: For Article Length -  It is distributed around 350 words, with very less being over 1K . For Bigram and Trigram Analysis: For Bigrams : ‘united states’, ‘new york’ & ‘tell cnn’ as the top 3. For Tri Grams : ‘president barack obama’, ‘express commentary solely’& ‘opinion express commentary’ are the top 3
Word cloud: The top three words in the wordcloud were found to be 'say', 'year', and 'one'. This represents that these words have the highest frequency of occurring in an article.
Topic Modeling:
Latent Dirichlet Allocation (LDA): LDA is used to extract topics from the dataset. The coherence score came out to be 0.58 for a maximum of 24 topics which was not so great for the BOW model and the processing time was high.
Non-negative matrix factorization (NMF): The NMF model was rerun using 21 topics to generate the document-topic matrix (W) and the topic-word matrix (H).The top 10 words for each of the 21 topics are extracted from the topic-word matrix to represent each topic meaningfully.A topic mapping is provided to assign descriptive labels to each topic, enhancing interpretability. The topics found were: "Family and Society", "Entertainment and Pop Culture", "US Politics", "Sports","Law and Crime", "Aviation and Accidents", "China and East Asia", "Korea and Geopolitics",  "Crime and Law Enforcement", "Health and Disease", "Middle East and Conflict", "Education and Academia", "Middle East Politics", "Syrian and Iraq Conflict", "Weather and Natural Disasters", "Sports Competitions", "Government and Protests", "Entertainment and Celebrity News", "Russia and Ukraine Conflict", "Economy and Business"& "Technology and Social Media" (Refer to Graph 6)
3.  Recommender System: Based on the mean vectors created and assignment to the documents, we are creating a recommender system that based on the user's query, takes out the cosine similarity between the query and the topic and then gives out the articles in that topic. Refer Graph 7 and 8
4. Practical Significance and real-world applications - Enhancing user engagement for digital media and news platforms. Also a content-based recommender system ensures that users receive personalized article suggestions, reducing bounce rates and increasing time spent on the platform. 
