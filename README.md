# 📘 Zipf's Law Analysis – Statistical Language Processing

## 🧠 Overview
This project explores **Zipf’s Law**, a fundamental principle in quantitative linguistics.  
Zipf’s Law states that the frequency of a word in a language is **inversely proportional to its rank**  
in the frequency table. In simple terms, the most common word appears about twice as often as  
the second most common, three times as often as the third, and so on.  

This statistical pattern is found across **all natural languages**, as well as in other domains such as  
city populations, website traffic, and software errors.

---

## 🧩 Project Description
The notebook performs a **statistical analysis of word frequencies** using a real text corpus  
(e.g., *War and Peace* by Leo Tolstoy, from Project Gutenberg).  
It demonstrates the validity of Zipf’s Law and extracts additional linguistic insights.

### 🔍 Key Components:
1. **Text Preprocessing**  
   - Loads and cleans a large text file.  
   - Converts to lowercase and tokenizes words using regular expressions.  

2. **Word Frequency Analysis**  
   - Counts occurrences of each word and assigns rank.  
   - Displays a log–log plot comparing actual frequencies with the ideal Zipf curve.  

3. **Rank × Frequency Product**  
   - Tests Zipf’s Law numerically by showing whether the product `rank × frequency`  
     remains approximately constant.  

4. **Vocabulary Coverage (90%)**  
   - Calculates how many of the most frequent words are needed to cover 90% of the text.  
   - Visualized as a cumulative coverage curve with a red 0.9 threshold line.  

5. **Word Co-occurrence Network**  
   - Builds an undirected graph linking words that appear next to each other.  
   - Identifies the “core language” — words with the highest number of neighbors,  
     typically functioning as grammatical connectors.

---

## 📈 Results
- The log–log distribution of word frequency closely follows **Zipf’s Law**.  
- A small fraction of words (e.g., ~2,500) accounts for 90% of the entire text.  
- The co-occurrence network highlights the structural backbone of the language,  
  showing highly connected functional words such as *and*, *the*, *of*, *to*, etc.

---

## 🛠️ Technologies Used
- **Python 3**
- **pandas**, **matplotlib**, **networkx**, **collections**, **re**

---

## 📚 References
- Zipf, G. K. (1949). *Human Behavior and the Principle of Least Effort.* Addison-Wesley.  
- Project Gutenberg: [https://www.gutenberg.org/ebooks/2600](https://www.gutenberg.org/ebooks/2600)

