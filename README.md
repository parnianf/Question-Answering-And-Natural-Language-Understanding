# Question-Answering-And-Natural-Language-Understanding


## Part 1: Question Answering (QA)

This part includes the implementation of a `BERT-based` model which returns “an answer”, given a user question and a passage which includes the answer of the question. For this question answering task, You should use the Persian datasets like `SQuAD`. You start with the `BERT-base` pretrained model `bert-base-parsbert-uncased` and fine-tune it to have a question answering task.

One of the fundamental objectives of artificial intelligence is the development of question-answering systems (QA). Deep Learning (DL) approaches have led to significant improvements in QA systems. Despite having excellent QA performance, DL needs a sizable amount of annotated data for training. For the QA work, many annotated datasets have been created; the majority of them are only in English and models doesn’t work on Persian Language. So we propose four models on three different datasets, PQuad, PersianQA, and ParsSquad, in order to answer the requirement for a high-quality QA dataset in the Persian language. Finally, we combine datasets from PersianQA and PQuad to create our final model.

The standard final project is to work on modifying and extending a neural question answering system. We use available Persian BERT (`ParsBERT`) and `ALBERT` (`ALBERT-Persian`).

In this part we should Train 4 question answering models individually for both `BERT` and `ALBERT` model:
1. `PQuAD` QA model (use PQuAD dataset)
2. `PersianQA` QA model (use PersianQA dataset)
3. `ParSQuAD` QA model (use ParSQuAD dataset)
4. `PQuAD` and `PersianQA` QA model (use mix of PQuAD and PersianQA
datasets)

#### Dataset
We are given three datasets as part of the **Machine Reading for Question** Answering (`MRQA`): 
1. [PQuAD](https://arxiv.org/abs/2202.06219)
2. [PersianQA](https://github.com/sajjjadayobi/PersianQA)
3. [ParSQuAD](https://github.com/NeginAbadani/ParSQuAD)

## Part 2: Natural Language Understanding (NLU)

**Intent detection** and **slot filling** are the main tasks to solve when approaching the problem of **Natural Language Understanding (NLU)** in a **conversational system**. The two tasks are used to obtain a structured representation of the meaning of the utterance, so that it can be processed by a computer. Intent detection deals with identifying the overall meaning of the sentence. It is modeled as a classification problem, in which we receive an input utterance and we have to classify it as having one intent from a group of known intents. The available intents correspond to the actions that the conversational model can perform, such as adjusting the temperature, controlling the media center or turning the lights on/off in the case of a home assistant. On the other hand, slot filling is modeled as a sequence labelling problem, whose purpose is to take the utterance and determine which words **indicate relevant information for the intent**. These slots contain supplementary information about the action and correspond to the parameters of the action.


The **task-oriented dialogue system** is the basis of virtual assistants like **Alexa**, **Siri**,
**Cortana**, and Portal has been increasingly used in modern society; users interact
with them across different domains to complete diverse tasks and achieve their
specific goals.
A key component of these task-oriented dialogue systems is Natural Language
Understanding (NLU) which aims to **derive the intent** of users and **fill the value for
the slots** of the utterance. For example, in the utterance "Play a chant by Mj Cole",
a dialogue system should correctly identify that the user's intention is to give a
command to play a song, and that Mj Cole is the artist name that the user would
like to listen.

#### Dataset
[MASSIVE](https://github.com/alexa/massive) is a parallel dataset of **> 1M** utterances across 51 languages with annotations for the Natural Language Understanding tasks of intent prediction and slot annotation. Utterances span **60 intents** and include **55 slot** types. **MASSIVE** was created by localizing the **SLURP** dataset, composed of general Intelligent Voice Assistant single-shot interactions.
In this assignment, we are to use Farsi Dataset (**fa-IR.jsonl**). This Json file contains train, dev and test sets.

