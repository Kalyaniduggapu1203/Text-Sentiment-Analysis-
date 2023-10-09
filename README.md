import matplotlib.pyplot as plt
from wordcloud import WordCloud

# Assuming 'cleaned_text' is a list of cleaned text data
text = ' '.join(cleaned_text)

wordcloud = WordCloud(width=800, height=400, max_words=20, background_color='white').generate(text)

plt.figure(figsize=(10, 5))
plt.imshow(wordcloud, interpolation='bilinear')
plt.axis('off')
plt.title('Top 20 Most Frequent Words')
plt.show()
