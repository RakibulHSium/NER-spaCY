# Custom Named Entity Recognition with spaCy
Methodology used to create and train a custom Named Entity Recognition (NER) model using spaCy.

## Table of Contents

- [Methodology](#methodology)
  - [Data Collection](#data-collection)
  - [Preprocessing](#preprocessing)
  - [Data Annotation](#data-annotation)
  - [Model Selection and Configuration](#model-selection-and-configuration)
  - [Training Data Preparation](#training-data-preparation)
  - [Training](#training)
  - [Evaluation](#evaluation)
  - [Data Visualization](#data-visualization)

## Methodology

### Data Collection

| Step              | Description                                      |
|-------------------|--------------------------------------------------|
| Data Collection   | Dataset obtained from Kaggle: [medical-ner](https://www.kaggle.com/datasets/finalepoch/medical-ner) |
|                   | Kaggle dataset provided the source data for NER training. |

### Preprocessing

| Step              | Description                                      |
|-------------------|--------------------------------------------------|
| Preprocessing     | Utilized spaCy for tokenization and preprocessing. |
|                   | The content of the dataset was tokenized and prepared for training. |

### Data Annotation

| Step              | Description                                      |
|-------------------|--------------------------------------------------|
| Data Annotation   | Annotations extracted from the data included start and end positions and associated labels. |
|                   | Labels correspond to different named entity categories (e.g., "PATHOGEN," "MEDICINE," "MEDICALCONDITION"). |

### Model Selection and Configuration

| Step              | Description                                      |
|-------------------|--------------------------------------------------|
| Model Selection   | spaCy NER model ("en_core_web_lg") loaded as a starting point for customization. |
| Model Customization | Adaptations made to the model to suit the specific NER task and named entity labels. |

### Training Data Preparation

| Step              | Description                                      |
|-------------------|--------------------------------------------------|
| Data Preparation  | Data transformed into a format suitable for spaCy's training process. |
|                   | Each training example consisted of the original text and associated entity annotations. |

### Training

| Step              | Description                                      |
|-------------------|--------------------------------------------------|
| Training          | spaCy model fine-tuned on the prepared data, optimizing the NER components. |
|                   | Iterations over the data to train the model to recognize specified named entities. |

### Evaluation

| Step              | Description                                      |
|-------------------|--------------------------------------------------|
| Evaluation Metrics | Criteria defined to assess the performance of the trained model. |


### Data Visualization

| Step              | Description                                      |
|-------------------|--------------------------------------------------|
| Data Visualization | spaCy `displacy` library used to visualize NER results. |

The above methodology outlines the key steps and procedures undertaken to create and train the custom NER model.
