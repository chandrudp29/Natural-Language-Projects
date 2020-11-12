# Natural-Language-Processing overview
![](https://www.xenonstack.com/images/blog/2019/12/evolution-of-nlp-xenonstack.png)

Natural language processing is a subset of Artificial intelligence that helps computers to understand, interpret, and utilize the human languages. NLP allows computers to communicate with peoples using human languages. NLP also provides computers with the ability to read text, hear speech, and try to intrepret it. NLP draws several disciplines, including Computational linguistics and computer science, as this attempts to fill the gap in between human and computer communication.
NLP breaks down language into shorter, more basic pieces, called tokens(period, words, etc), and attempts to understand the relationships of tokens. This approach often uses higher-level NLP features, such as:
- Sentiment analysis: It identifies the general mood, or subjective opinions, which is stored in large amount of texts, It is more useful for opinion mining.
- Contextual Extraction: Extract structured data from text-base sources.
- Text-to-Speech and Speech-to-text: It transforms the voice into text and vice a versa.
- Document Summarization: Automatically creates a synopsis, condensing large amounts of text.
- Machine Translation: Translates the text or speech of one language into another language.

## Text Preprocessing
Supose we have textual data available, we need to apply many of pre-processing steps to the data to transform those words into numerical features that work with machine learning algorithms.
The pre-processing steps for the problem depend mainly on the domain and the problem itself.We don't need to apply all the steps for every problem.
![](https://miro.medium.com/max/2050/1*ES5bt7IoInIq2YioQp2zcQ.png)
## Stemming
From Stemming we will process of getting the root form of a word. Root or Stem is the part to which inflextional affixes(like -ed, -ize, etc) are added. We would create the stem words by removing the prefix of suffix of a word. So, stemming a word may not result in actual words.

For Example: Mangoes ---> Mango

         Boys ---> Boy

         going ---> go
If our sentences are not in tokens, then we need to convert it into tokens. After we converted strings of text into tokens, then we can convert those word tokens into their root form. These are the Porter stemmer, the snowball stemmer, and the Lancaster Stemmer. We usually use Porter stemmer among them.
## Lemmatization
As stemming, lemmatization do the same but the only difference is that lemmatization ensures that root word belongs to the language. Because of the use of lemmatization we will get the valid words. In NLTK(Natural language Toolkit), we use WordLemmatizer to get the lemmas of words. We also need to provide a context for the lemmatization.So, we added pos(parts-of-speech) as a parameter.
## Parts of Speech (POS) Tagging
The pos(parts of speech) explain you how a word is used in a sentence. In the sentence, a word have different contexts and semantic meanings. The basic natural language processing(NLP) models like bag-of-words(bow) fails to identify these relation between the words. For that we use pos tagging to mark a word to its pos tag based on its context in the data. Pos is also used to extract rlationship between the words.
![](https://slideplayer.com/slide/5260592/16/images/2/What+is+POS+tagging+Tagged+Text+Raw+Text+POS+Tagger.jpg)
## Chunking
Chunking is the process of extracting phrases from the Unstructured text and give them more structure to it. We also called them shallow parsing.We can do it on top of pos tagging. It groups words into chunks mainly for noun phrases. chunking we do by using regular expression.
![](https://www.tutorialkart.com/wp-content/uploads/2017/06/chunker_ex.png)
![](https://encrypted-tbn0.gstatic.com/images?q=tbn%3AANd9GcSqPsHKdul3gHVJvIVc9_98nIjzAtbFrY_x6Q&usqp=CAU)
## Named Entity Recognition
It is used to extract information from unstructured text. It is used to classy the entities which is present in the text into categories like a person, organization, event, places, etc. This will give you a detail knowledge about the text and the relationship between the different entities.
![](https://i.stack.imgur.com/MD0LG.png)
## Regex
As you're a software developer, you have probably encountered regular expressions many times and got consufed many times with these daunting set of characters grouped together like this:
![](https://miro.medium.com/max/1374/1*ZXTb1lt1LYysa1yki__0Aw.gif)

A Regex or we called it as regular expression, it is a type of object will help you out to extract information from any string data by searching through text and find it out what you need.Whether it's punctuation, numbers, letters, or even white spaces, RegEx will allow you to check and match any of the character combination in strings.
![](https://i.imgur.com/KmCtFLP.png)
## Text normalization
In the tect pre-processing highly overlooked step is text normalization. The text normalization means the process of transforming the text into the canonical(or standard) form. Like, "ok" and "k" can be transformed to "okay", its canonical form.And another example is mapping of near identical words such as "preprocessing", "pre-processing" and "pre processing" to just "preprocessing".

Text normaliztion is too useful for noisy textssuch as social media comments, comment to blog posts, text messages, where abbreviations, misspellings, and the use out-of-vocabulary(oov) are prevalent.
![](https://cdn-images-1.medium.com/max/1600/1*e7Y-Rbxky5i2U6awCQILVQ.png)

Source : Internet 
