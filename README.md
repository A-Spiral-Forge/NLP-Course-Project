# Important Information Extraction From Short Text Messages
This project focuses on extracting important information from short text messages. The goal is to develop a system that can automatically identify and extract key details from the messages to facilitate further analysis or action.

## Dataset
The dataset used in this project is the [SMS Dataset](https://www.kaggle.com/datasets/dshah1612/sms-data) from Kaggle. It contains 59.4k unique text messages in English. From this I have used 110 messages for training and 60 messages for testing. I have created the annotated dataset by hand. The dataset is available in the `annotations_new.json` file.

## Approach
The approach used in this project is to train a Named Entity Recognition (NER) model using the [spaCy](https://spacy.io/) library. The model is trained on the annotated dataset and then used to extract the entities from the test messages. The entities extracted are then compared with the ground truth entities to calculate the precision, recall and F1 score.

## Technologies Used
* Python 3.7
* spaCy 3.5.1
* numpy 1.24.2
* pandas 2.0.0
* regex 2021.4.4
* tqdm 4.65.0

## How to Run
To run the project, follow the steps below:
1. Clone the repository using `git clone https://github.com/A-Spiral-Forge/NLP-Course-Project.git`.
2. Navigate to the project directory using `cd NLP-Course-Project`.
3. Install the dependencies using `pip install -r requirements.txt`.
4. Run the jupyter notebook `nlp-course-project.ipynb`.

## Results
The results obtained are as follows:
* Precision: 79.03
* Recall: 83.05
* F1 Score: 75.38
* Score: 0.79

## Future Work
The results obtained are slightly good. This is because the dataset is very small sue to memory constraint. The model can be improved by using a larger dataset. Also, the model can be improved by using a more sophisticated model like BERT.

## Contributors
* [Abhay Parihar](https://github.com/A-Spiral-Forge/)