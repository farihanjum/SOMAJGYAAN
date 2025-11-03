# SOMAJGYAAN: A Dataset for Evaluating LLMs on Bangla Culture, Social Knowledge, and Low-Resource Language Adaptation

[![Paper](https://img.shields.io/badge/ACL%20Anthology-IJCNLP%20AACL%20Findings%202025-EE161F)]()
[![Dataset](https://img.shields.io/badge/%F0%9F%A4%97%20Dataset-SOMAJGYAAN-ffc107?color=ffc107&logoColor=white)](https://huggingface.co/datasets/farihashifa/SOMAJGYAAN)
[![GitHub](https://img.shields.io/badge/GitHub-Code-blue?logo=github)](https://github.com/farihanjum)

[Fariha Anjum Shifa*](https://github.com/farihanjum), Muhtasim Ibteda Shochcho*, Abdullah Ibne Hanif Arean*, Mohammad Ashfaq Ur Rahman, AKM Moshiur Rahman Mazumder, Ahaj Mahhin Faiak, Md Fahim, M Ashraful Amin, Amin Ahsan Ali, AKM Mahbubur Rahman

*Equal Contribution

---

## 📊 Dataset Overview

**SOMAJGYAAN** presents a robust Bangla multiple-choice dataset that reflects the knowledge of underrepresented regions such as Bangladesh. It consists of **4,234 questions** drawn from Bangladesh's National Curriculum and Global Studies textbooks, covering a wide range of domains including **History, Geography, Economics, Social Studies, Politics and Law, and Miscellaneous topics**.

---



## 🎯 Key Features

- ✅ **4,234 culturally relevant questions** covering Bangladeshi curriculum
- ✅ **Five difficulty levels** with Cohen's Kappa = 0.71 inter-annotator agreement
- ✅ **~12,640 unique answer options** ensuring diverse vocabulary coverage
- ✅ **Seven academic categories** spanning History, Geography, Economics, Politics, Social Studies, Law, and Miscellaneous
- ✅ **Benchmark for low-resource language evaluation**

---

### Difficulty Level Distribution

| Difficulty Level | Description |
|------------------|------------|
| **Level 1** | Easy - Direct factual recall |
| **Level 2** | Moderate - Basic reasoning |
| **Level 3** | Moderate-High - Fact + reasoning |
| **Level 4** |  High - Context-based single-hop |
| **Level 5** |Very High - Context-based multi-hop |
### Q&A Statistics

| Statistic | Questions (Q) | Answers (A) |
|-----------|---------------|-------------|
| **Mean Word Count** | 19.25 | 2.15 |
| **Max Word Count** | 83 | 10 |
| **Min Word Count** | 6 | 1 |

---




### Example Data Point
```python
{
  "Question": "১৯৫২ সালে পূর্ববাংলার মুখ্যমন্ত্রী কে ছিলেন?",
  "Category": "History",
  "Difficulty": 2,
  "A": "খাজা নাজিমুদ্দিন",
  "B": "নুরুল আমিন",
  "C": "আতাউর রহমান খান",
  "D": "আবু হোসেন সরকার",
  "Answer": "B",
}
```

**Translation:** Who was the Chief Minister of East Bengal in 1952?  
**Correct Answer:** B - নুরুল আমিন (Nurul Amin)

---

## 🔬 Experimental Findings

### Model Performance Overview

Our experiments with both open-source and closed-source LLMs reveal:

1. **Closed-source models outperform open-source models** across all categories
   - Gemini 2.0 Flash: 73% accuracy
   - GPT-4o: 69% accuracy
   - Claude 3.7: 64% accuracy

2. **Open-source model performance**
   - DeepSeek-R1-Distill-14B: 56% (best open-source)
   - Phi 4: 52%
   - Qwen 2.5-7B: 47%

3. **Fine-tuning improves open-source models** by 5-10% but still lags behind closed-source
   - Demonstrates need for culturally grounded training data

4. **Category-specific challenges**
   - Law and Politics categories are most challenging
   - Economics and History show better performance

5. **Difficulty scaling**
   - Performance degrades significantly at Level 4-5 (context-based multi-hop reasoning)

---

## 📖 Dataset Creation

### Data Sources

Questions were curated from:
- **Bangladesh National Curriculum** textbooks (Classes VI-X)
- **Global Studies** educational materials
- **Panjeree Guide Books**


### Data Quality

- ✅ Grammar and spelling verified using Avro Keyboard and Bangla Spell Checker
- ✅ Duplicate removal
- ✅ Logical consistency checks
- ✅ Cultural appropriateness validation

---

## 📄 Citation

To be added later

## 📧 Contact

- **Correspondence:** fahimcse381@gmail.com
- **Institution:** University of Dhaka, Center for Computational & Data Sciences
- **GitHub:** [farihanjum](https://github.com/farihanjum)

---

## 📜 License

Later.

---

## 🔗 Related Resources

<!-- - 📄 [Paper (ACL Anthology)](https://aclanthology.org/2024.findings-emnlp.859/) -->
- 🤗 [Hugging Face Dataset](https://huggingface.co/datasets/farihashifa/SOMAJGYAAN)
- 💻 [GitHub Repository](https://github.com/farihanjum)

---

<div align="center">

**Made with ❤️ for advancing Bangla NLP**

**সমাজজ্ঞান (SOMAJGYAAN) - Social Knowledge in Bangla**

</div>
