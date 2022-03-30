# Abstract
Natural Language Processing models are the keystone to enabling computers to learn human languages and respond similarly. We use this more and more in our daily activities, for example asking Google or Siri for a stock market update, weather report, top news stories.

The first steps involve machine learning on text data, after which the text gets transformed into high-dimensional numerical vectors or embeddings. At present, the number of resulting dimensions can range from hundreds to thousands. After the text data gets converted into numbers and vector space, we can pass it on down the machine learning pipeline.


# Methodology
While it is easy to understand and visualize two or three dimensions, it becomes impossible with the high-dimensional space of text embeddings. Google and Facebook have a couple of the current state-of-the-art language embedding algorithms out there. Google’s Universal Sentence Encoder which produces 512 embedding dimensions while Facebook’s Infersent churns out a whopping 4,096 dimensions!

One of the ways of trying to visualize high-dimensional data is a tool called t-distributed Stochastic Neighbor Embedding or t-SNE. With t-SNE, we can look at the embeddings in two or three dimensional space. This is useful for checking if clusters existed in the data.

My analysis scope:
* apply Google's Universal Sentence Encoder and get 512 embedding dimensions for each essay
* apply t-Stochastic Neighbor Embedding (t-SNE) algorithm and reduce high-dimensional embeddings down to 2D
* check 2D cluster visualizations by limiting essay lengths to first 30, 70 and 140 characters
* explore presence of clustering along dating app user features like age, gender and pet preferences

<p align="center">
  <img src="https://github.com/gracehikes/proj_dating_essays_tSNE_clusters/blob/main/images/essay%20lengths%2030%2070%20140%20example.png" width=60% height=60%>
</p>


# Results
The table below summarizes the measured effects of social media daily use on the young people's survey responses. Among the young people who reported spending 1-3 hours on a normal school day chatting with their friends on social media i.e. treatment group A, the effects on how they felt on the 6 indicators were very small (ranging from -0.09 change in score when asked about their friends, to +0.20 for appearance) and generally not statistically significant.

When we reviewed the responses from “power users” of social media i.e. the young people who spent 4 or more hours per normal school day on social media (treatment group B), the estimated effects on well-being scores were all movement toward the more unhappy end of the 1-7 emoticon scale. Three out of the six indicators of mental well-being exhibited statistical significant treatment effects: feelings about school work (+0.37, p=0.02), school they went to (+0.69, p<0.00001), and life as a whole (+0.49, p=0.0004). 

<p align="center">
  <img src="https://github.com/gracehikes/proj_dating_essays_tSNE_clusters/blob/main/images/tSNE%20visual%20cluster%20by%20age.png" width=90%>
</p>

<p align="center">
  <img src="https://github.com/gracehikes/proj_dating_essays_tSNE_clusters/blob/main/images/tSNE%20visual%20cluster%20by%20age.png" width=80% height=90%>
</p>


# More Details
Full report found [here](/_project-report---youth-and-social-media---grace-yang.pdf).
