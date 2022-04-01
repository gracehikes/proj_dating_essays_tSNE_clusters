
# Abstract
Natural Language Processing models are the keystone to enabling computers to learn human languages and respond similarly. We use this more and more in our daily activities, for example asking Google or Siri for a stock market update, weather report, top news stories.

The first steps involve machine learning on text data, after which the text gets transformed into high-dimensional numerical vectors or embeddings. Google and Facebook have a couple of the current state-of-the-art language embedding algorithms out there. Google’s Universal Sentence Encoder which produces 512 embedding dimensions while Facebook’s Infersent churns out a whopping 4,096 dimensions! While it is easy to understand and visualize two or three dimensions, it becomes impossible with the high-dimensional space of text embeddings. 

One of the ways of trying to visualize high-dimensional data is a tool called t-distributed Stochastic Neighbor Embedding (t-SNE). With t-SNE, we can look at a representation of the high-dimensional embeddings in the two or three dimensional space. In the t-SNE algorithm paper ([L.van der Maaten and G. Hinton, 2008](https://www.jmlr.org/papers/volume9/vandermaaten08a/vandermaaten08a.pdf?fbclid=IwA)), we can see 10 distinct clusters after high-dimensional embeddings for MNIST handwritten digits 0-9 were passed through the t-SNE algorithm and plotted in two dimensions.


# Methodology
My analysis scope:
* apply Google's Universal Sentence Encoder and get 512 embedding dimensions for each essay
* apply t-SNE algorithm and reduce high-dimensional embeddings from 512 down to 2
* limit essay lengths to first 30 / 70 / 140 characters and look for clusters in 2-dimensional space 
* explore presence of clusters along features like dating app user's age, gender and pet preference

<p align="center">
  <img src="https://github.com/gracehikes/proj_dating_essays_tSNE_clusters/blob/main/images/essay%20lengths%2030%2070%20140%20example.png" width=70%>
</p>


# Results
It appeared men and women write in very similar manner for their dating self-summaries - see visualizations below. There were no clear clusters to be visualized by age of the dating singles. For pet preference, I also did not see separate clusters for dog-lovers versus cat-lovers. 

The longer the essay snippets used to generate embeddings, the closer the visualized data points start to merge to one another as shown in the diagrams below. The ability to see clusters (if any) favored shorter essay lengths.

<p align="center">
  <img src="https://github.com/gracehikes/proj_dating_essays_tSNE_clusters/blob/main/images/tSNE%20visual%20cluster%20by%20gender.png" width=95%>
</p>


# More Details
Full report found [here](/graceyang_final_thesis_filed.pdf).

