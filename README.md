### Knowledge-enhanced Bilingual Textual Representations for Cross-lingual Semantic Textual Similarity

# Introduction

Cross-lingual representations learning receives high attention recently, but is still restricted by the availability of parallel data. 

In this work we propose a method jointly embed **texts and KB entities** on comparable data. Different to other cross-lingual representations learning methods, our method can apply on weakly-supervised cross-lingual data (articles, paragraphs, and texts), and is still able to capture cross-lingual information well. Our method is validated on **Semantic Textual Similarity (STS)** task, including mono-lingual and cross-lingual datasets of SemEval-14 and SemEval-17.

# Inspiration

Existing STS methods are incapable to assess the semantic similarity of cross-lingual texts. In mono-lingual setting, the dissimilarity of text pairs can be graded by supervised models (from 0 to 5).

It is easy to assess the similarity of text pairs by fitting models on annotated similarity labels. But the cost to annotate data is expensive. In order to reduce the requirement of supervised data, we propose a method to generate comparable texts, and train cross-lingual sentence embeddings on the data generated.

To address the issues mentioned above, we propose a framework that integrates the information of text and Knowledge Base (KB) entities so as to model cross-lingual semantic relatedness of texts. Different to STS tasks, our method is capable to **assess the relatedness between imbalanced texts**.

---

# Framework

The overall framework is as shown in **Fig. 1**, including three modules: (1) mono-lingual word, entity learning, (2) cross-lingual text regularizer, and (3) joint learning of text and entity.

![framework.png](framework.png =821x506)
<center style="font-size:14px;color:#C0C0C0;text-decoration:underline">Fig. 1: Framework of joint model.</center>

The model is based on Skip-Gram algorithm. In our method, we train all words, and KB entities embeddings jointly, including mono-lingual and cross-lingual embeddings. 

---

# Released Embeddings

In this work, we choose three languages (English, Chinese, Spanish) as our main research languages. All embeddings are 300d and can be downloaded in the following links.

Language | 1st  | 2nd
 :---: | :---: | :---:
  En-Zh | [En]() | [Zh]()
  En-Es | [En]() | [Es]()
  
---

# Citation

If you found this work helpful, consider citing the work as:

``
@InProceedings{10.1007/978-981-15-0118-0_33,
author="Lu, Hsuehkuan
and Cao, Yixin
and Lei, Hou
and Li, Juanzi",
editor="Cheng, Xiaohui
and Jing, Weipeng
and Song, Xianhua
and Lu, Zeguang",
title="Knowledge-Enhanced Bilingual Textual Representations for Cross-Lingual Semantic Textual Similarity",
booktitle="Data Science",
year="2019",
publisher="Springer Singapore",
address="Singapore",
pages="425--440",
isbn="978-981-15-0118-0"
}
``

---

