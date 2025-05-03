## ✅ **Assignment 2 Summary: Topic Modeling with LDA**

### 📌 **Objective**:

To extract latent topics from a corpus of 10 documents using **Latent Dirichlet Allocation (LDA)** and gain insights from topic distributions.

---

### 🔍 **Task 1: Data Exploration & Preprocessing**

* **Data**: A small dataset of 10 short documents discussing various global issues and technologies.
* **Steps**:

  * Removed punctuation and digits.
  * Tokenized, lowercased, removed stopwords.
  * Applied **WordNet Lemmatization**.
* **Corpus & Dictionary**: Created using `gensim` from tokenized data.

---

### 🧹 **Preprocessing Output (Sample)**:

* Text converted into meaningful tokens such as:

  ```
  ['stock', 'market', 'experience', 'volatility', 'recent', 'month']
  ```

---

### 🧠 **Task 2: Topic Generation Using LDA**

* **Model**: `LdaModel` from `gensim`
* **Parameters**:

  * `num_topics = 5`
  * `passes = 10`
  * `alpha = 'auto'` (adaptive learning)

---

### 📊 **Top Words per Topic (After Parsing)**

| Topic # | Top Words                                           |
| ------- | --------------------------------------------------- |
| 0       | industry, platform, digital, streaming, world       |
| 1       | industry, future, treatment, platform, economy      |
| 2       | attention, critical, immediate, climate, global     |
| 3       | cybersecurity, become, ongoing, integrated, concern |
| 4       | industry, automobile, uncertainty, future, stock    |

---

### 💡 **Insights & Interpretations**

1. **Topic 0 – Digital Media & Global Reach**
   Keywords like *digital*, *streaming*, *platform*, and *world* suggest this topic centers around **digital transformation and global platforms**.

2. **Topic 1 – Economic Growth & Healthcare Innovation**
   The mix of *treatment*, *platform*, *economy*, and *future* indicates a focus on **emerging technologies in healthcare and economic growth**.

3. **Topic 2 – Climate Change Awareness**
   High-weighted terms like *critical*, *climate*, *global*, *immediate* show strong alignment with **urgent environmental concerns**.

4. **Topic 3 – Cybersecurity as a Growing Concern**
   Words like *cybersecurity*, *integrated*, and *concern* point to a **rising focus on cybersecurity risks and solutions**.

5. **Topic 4 – Automotive Industry & Market Uncertainty**
   Terms like *automobile*, *uncertainty*, *stock* hint at **economic volatility affecting the auto industry**.

---

### 📈 **Conclusion**

The LDA model effectively extracted coherent topics reflecting real-world domains:

* Digital transformation
* Climate issues
* Cybersecurity
* Healthcare
* Economic uncertainty
