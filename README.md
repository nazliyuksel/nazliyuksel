- 👋 Hi, I’m @nazliyuksel
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
nazliyuksel/nazliyuksel is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import nltk
from nltk.tokenize import word_tokenize
from nltk.corpus import stopwords

# Ön gereksinimler
nltk.download('punkt')
nltk.download('stopwords')

# Örnek metin
text = "Doğal dil işleme, metinlerin analiz edilmesini sağlayan bir disiplindir."

# Tokenizasyon
tokens = word_tokenize(text)

# Stop kelimeleri çıkarma
stop_words = set(stopwords.words('turkish'))
filtered_tokens = [word for word in tokens if word.lower() not in stop_words]

print("Tokenized:", tokens)
print("Filtered:", filtered_tokens)
