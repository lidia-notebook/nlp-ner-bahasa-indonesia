# **Named Entity Recognition (NER) for Indonesian Text**

## **Project Overview**

This project focuses on building a Named Entity Recognition (NER) model for Indonesian text using multilingual BERT. The objective is to identify and classify entities such as person names, locations, and organizations from text data.

---

## **Business Understanding**

Named Entity Recognition (NER) helps transform unstructured text into structured information. This can support:

- Information extraction
- Customer support automation
- Social media monitoring
- News and document analysis
- AI-powered NLP applications

---

## **Dataset**

- **Dataset:** WikiANN Indonesian Dataset
- **Task:** Token Classification / Named Entity Recognition
- **Labels:** BIO tagging format (B-PER, I-PER, B-ORG, B-LOC, O, etc.)

---

## **Project Workflow**

1. Data Loading & Exploration  
2. Data Preprocessing  
3. Tokenization & Label Alignment  
4. Fine-Tuning Multilingual BERT  
5. Model Training & Evaluation  
6. Prediction & Inference  

---

## **Model**

- **Pretrained Model:** Multilingual BERT (mBERT)
- **Task Type:** Token Classification
- **Framework:** Hugging Face Transformers

---

## **Tools & Libraries**

- Python
- Pandas
- NumPy
- Hugging Face Transformers
- Datasets
- PyTorch
- Scikit-learn
- Matplotlib
- Google Colab

---

## **AI Ethics Considerations**

### **Data Security**

- WikiANN is fully public and sourced from Wikipedia
- No sensitive personal data (ID numbers, addresses) is present

### **User Privacy**

- No private communications or personal data used
- Anonymization recommended if deployed on real user-generated content

### **Bias Awareness**

| Bias Type | Description |
|---|---|
| Name bias | Western names may be recognized better than local Indonesian names |
| Topic bias | Performance may vary across political, cultural, and local news |
| Entity imbalance | `LOC` is more frequent than `ORG` in training data |

---

## **Recommendations for Improvement**

1. **Add more training data** — more diverse Indonesian text improves generalization  
2. **Include Date entity** — add custom annotated data for date recognition  
3. **Fine-tune on news data** — use articles from detik.com / kompas.com  
4. **Address name bias** — add more local Indonesian names in training data  
5. **Try IndoBERT** — `indobenchmark/indobert-base-p1` is pre-trained on Indonesian text  

---

## **References**

- [WikiANN Dataset](https://huggingface.co/datasets/unimelb-nlp/wikiann)
- [bert-base-multilingual-cased](https://huggingface.co/google-bert/bert-base-multilingual-cased)
- [HuggingFace Transformers](https://huggingface.co/docs/transformers)
- [seqeval](https://github.com/chakki-works/seqeval)

---

## **Author**

**Lidia**

- LinkedIn: [LinkedIn](https://linkedin.com/in/lidiapriskila)

---

## **License**

This project is licensed under the MIT License.
