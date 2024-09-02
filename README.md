# **MentalHelp**  
*14 million, semi-supervised, mental disorder detection data.*

---

## **Overview**

MentalHelp is a large-scale dataset designed for the detection of mental health disorders in social media, particularly on Reddit. With over **14 million** instances, this dataset offers researchers the ability to train and evaluate models in the mental health domain using semi-supervised learning techniques.

### **Key Features**
- **Large-Scale Data**: Over 14 million instances collected from Reddit.
- **Semi-Supervised Labeling**: Labels were generated using an ensemble of three models: flan-T5, Disor-BERT, and Mental-BERT.
- **Confidence Scores**: Each instance includes average confidence scores, enabling the selection of high-quality labeled data for training robust models.

---

## **Updates**

### **June 19th, 2024**

We are pleased to announce the release of approximately **33,000 samples**, each containing an **ID** and its corresponding **label**. The full dataset is available upon request, subject to a data usage agreement. The terms and conditions for accessing the full dataset will be provided in due course.

### **September 2nd, 2024**

We have now released **500,000 post IDs** with their associated labels. Although our intention was to release the entire dataset along with the content at once, we are currently constrained by the community guidelines of Reddit, which prevents us from doing so.

---

## **Benchmark Datasets**

MentalHelp integrates multiple publicly available datasets focused on mental health. Here are some of the key datasets included:

| **Dataset** | **Category** | **Source** | **Instances** |
|-------------|--------------|------------|---------------|
| depsev      | Depression   | Reddit     | 3,553         |
| datd        | Depression, Anxiety | Twitter | 5,550 |
| signdep     | Depression   | Reddit     | 16,632        |
| sdcnl       | Suicide      | Reddit     | 1,895         |
| sid         | Suicide      | Twitter    | 1,385         |
| dreaddit    | Stress       | Reddit     | 3,553         |

A total of **11 benchmark datasets** are used, covering a wide range of mental health issues including depression, anxiety, bipolar disorder, and suicidal ideation. The merged dataset comprises **163,839** instances.

---

## **Research and Evaluation**

MentalHelp has been used to evaluate various transformer models, demonstrating the effectiveness of specialized models in detecting mental health issues on social media. The models were trained and evaluated on the Google Colab Pro+ platform using Nvidia A100 GPUs.

### **Performance Highlights**
- **flan-T5** achieved the highest weighted F$_1$ score across multiple datasets.
- **Disor-BERT** and **Mental-BERT** also performed exceptionally well, particularly on task-specific datasets.
- GPT3.5-turbo, while not performing as well in zero-shot scenarios, showed improvement in few-shot settings.

---

## 📝 **Citation**

If you find this dataset useful in your research, we kindly ask you to cite our paper:

```bibtex
@inproceedings{raihan2024mentalhelp,
  title={MentalHelp: A Multi-Task Dataset for Mental Health in Social Media},
  author={Raihan, Nishat and Puspo, Sadiya Sayara Chowdhury and Farabi, Shafkat and Bucur, Ana-Maria and Ranasinghe, Tharindu and Zampieri, Marcos},
  booktitle={Proceedings of the 2024 Joint International Conference on Computational Linguistics, Language Resources and Evaluation (LREC-COLING 2024)},
  pages={11196--11203},
  year={2024}
}
