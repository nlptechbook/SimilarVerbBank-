# SimilarVerbBank: a dataset of similar verbs 

SimilarVerbBank is a dataset of similar verbs, which was programmatically generated on a relatively small text corpus formed from randomly chosen Wikipedia articles (plain text of about 8Mb in size, containing about 50K sentences). The dataset includes two files: semantic_similar_verbs.json and context_similar_verbs.json.  

**semantic_similar_verbs.json** contains a little less than a thousand records, each representing a verb along with a set of verbs semantically close (synonyms/antonyms or near) to it, of those that the algorithm was able to recognize in the corpus.   

**context_similar_verbs.json** contains slightly more than half a thousand verb sets. A set contains the verbs that are used with the key verb in a similar context in the sample corpus. The verbs in the same group may not be synonyms or antonyms but they are often used together with the same nouns. For example, verbs publish and cite do not mean the same, not opposite in meaning. However, they are often used in the same context. Say, you may publish an article and/or you may cite it. The verb sets here were formed with the [Apriori algorithm](https://www.oracle.com/news/connect/association-analysis-data-python-pandas.html) applied to the token groups generated using syntactic dependencies discovered in the text sentences. 

>You can ask us to generate a similar dataset on your text corpus. We'll be able to do it for a small fee. 
