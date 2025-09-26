# NLP Sentiment Twitter Analysis Using LDA Model
Building LDA model to analysis sentiment twitter. This code draws from several references and Kaggle's twitter sentiment dataset. FYI, this is the first NLP model I've tried to build :D observe imitate and modify hehe.

## Dependencies
- pandas
- matplotlib
- NLTK
- textblob
- gensim
- seaborn
- re
- warnings
- numpy
- pyLDAvis

To run this project, you will need to add the following requirements to your project.

```bash
!pip install -r requirements.txt
```
To install the pyLDAvis library, follow this code:

```bash
!pip install pyLDAvis
```

## Storyboard
In this project, I conducted sentiment analysis on Twitter data to gain deeper insights into public opinion, especially around topics that trigger negative reactions. The process began with thorough data preparation and text cleaning—removing unnecessary columns, converting all text to lowercase, stripping out non-alphanumeric characters and numbers, and handling missing values to make the dataset consistent and ready for analysis.

For sentiment classification, I used the TextBlob library to calculate polarity scores and labeled each tweet as positive, negative, or neutral based on set thresholds. The distribution visualization revealed a significant portion of negative tweets, which became the main focus. A Word Cloud generated from negative tweets highlighted frequently used terms such as “nvidia,” “fuck,” “shit,” “game,” and “fucking,” pointing to recurring frustrations among users.

To dive deeper, I applied Latent Dirichlet Allocation (LDA) topic modeling exclusively on the negative tweets after filtering out stopwords. Five main topics emerged, with several directly targeting NVIDIA and its products (like “RTX” and “GPU”), often coupled with harsh language and demands for fixes. Other topics reflected poor gaming experiences, user frustration, and general dissatisfaction. Overall, the findings clearly show that NVIDIA is at the center of negative discussions, closely followed by issues related to gaming experiences.

These insights help uncover the core drivers of negative sentiment and provide a solid foundation for shaping better user experiences and brand communication strategies on social media.

