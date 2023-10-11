# Task 2C : Building a Closed and Extractive Question and Answer Language model based on provided Context

The goal of this task is to experiment and discover an language model that is suitable for the task of context based extractive question answering. The evaluation should be done on the validation dataset using Metrics like Exact Match(EM) smd F1 score. Calculate the F1 score for the whole validation set by aversging the score for each context,question and answer triplet.

> The NewsQA Dataset and the evaluation metrics along with some other useful links are provided in the references

The baseline model provided is itself od very high standard due to the fact that we are fine-tuning a RoBerta model which has not just been pretrained on normal text with MLM and NSP objectives but also pretrained with the objective of Extractive Context based QnA on the standard SQuaD dataset. We futher fine tune it on the NewsQA dataset for even better perfomance on the newsQA dataset. 

Firstly, It should be very evident by going through the notebook that the hyperparameters are poorly chosen and little fine-tuning could help boost the performance.

Different forms of experimentation and architectural model building are encouranged irrelevant of the performance of the model. Novel Ideation or Smart Experimentaion is highly appreciated.


## References :
- [Already Attached in the Baseline notebook](https://colab.research.google.com/drive/1WxGxCFE_1cESJ02baaBY-HBHmGjSlxJx?usp=sharing#scrollTo=JBKY-irY25_F)
- [The NewsQA dataset on Hugging face](https://huggingface.co/datasets/lucadiliello/newsqa)
- [What is NewsQA dataset](https://www.microsoft.com/en-us/research/project/newsqa-dataset/)
- [Roberta-FineTuned on SQuaD](https://huggingface.co/deepset/roberta-base-squad2)
- [Fine Tuning on Custom Data](https://huggingface.co/transformers/v3.2.0/custom_datasets.html#question-answering-with-squad-2-0)
- [Evaluation Metrics](https://qa.fastforwardlabs.com/no%20answer/null%20threshold/bert/distilbert/exact%20match/f1/robust%20predictions/2020/06/09/Evaluating_BERT_on_SQuAD.html#F1)
