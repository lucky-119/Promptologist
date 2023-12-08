# Promptologist
Large Language Model(LLM) for Medical Query Resolution

## 11-785 Introduction to Deep Learning Course Project
  + Lakshay Arora (lakshaya)
  + Aryan Singhal (aryans)
  + Aakriti Kinra (akinra)
  + Aditi Patil (apatil2)

## Code Organization
```
├── checkpoints
│   ├── Best_Baseline_Checkpoint
│   ├── Best_Mode_Checkpoint
│   ├── Running_Mode_Checkpoint
├── code
│   ├── model
│   │   ├── Promptologist.ipynb
│   ├── translate.ipynb
├── data
│   ├── test.json
│   ├── testFinal.txt
│   ├── valid.txt
│   ├── trainFinal.txt(not added, file too big)
├── docs
│   ├── Promptologist_IDL_MidTerm_Report.pdf
│   ├── Promptologist_Final_Report.pdf
```

## Description
Promptologist is the Course Project for our [11-785 Introduction to Deep Learning](https://deeplearning.cs.cmu.edu/F23/index.html#:~:text=the%20calendar%20first.-,OH%20Calendar,-%3A%20The%20Google) Course for Fall 2023. It is a specialized Generative Pre-trained Transformer (GPT) tailored exclusively for the medical domain. 

## Goals

- We aim to build a robust large language model trained on medical dialogue that resolves patients queries.
- We aim to work on making it compact to save costs and compute and increase the accessibility to our users.
- The goal is to perform model distillation on a Large Language Model specifically in the field of medicine. 

## Constraints

Our problem is specifically restrained to the field of Medical Consultation and Patient query resolution.

## Model Architecture

We tried a various model architectures including Ngrams, Multi head attention, LSTMs and CNNs and found the N-Gram model with Multi-Head Attention with Convolutional Layers to give the best results

## Hardware

We trained the model on an NVIDIA Tesla T4 using Google Cloud Platform.

## Dataset

Our data includes English Patient-Doctor conversations and Chinese Patient-Doctor conversations converted to English. https://huggingface.co/datasets/shibing624/medical

## Data Preprocessing

+ Convert data from Chinese to English data using Google Translate.
+ Convert JSON Patient-Doctor conversations to line seperated texts.

## Evaluation Metric

+ BERT Score

## Loss Function
+ Cross-Entropy Loss function

## Deliverables

+ [Midterm Report](https://github.com/lucky-119/Promptologist/blob/main/docs/Promptologist_IDL_MidTerm_Report.pdf)
+ [Final Report](https://github.com/lucky-119/Promptologist/blob/main/docs/Promptologist_Final_Report.pdf)
+ [Project Video](https://www.youtube.com/watch?v=7ZeoCHyi4zY)

## Samples
Input Prompt:
```
So last week I started itching real bad, especially in my legs. I started noticing some bruising (and there were a lot of bruises, BIG bruises) where I scratched. I didnt think I was scratching so hard and Ive never bruised like this before whenever Ive had skin problems where I needed to scratch. Now, I found a lump in my upper thigh and its the size of a quarter. I can only notice it when I touch it and it feels like Im pressing against another bruise. However nothing has appeared on the skin which is leading me to believe its beneath the skin. Any ideas on what it could be?
```
Output:
```
Such as a CAss is out a rall laparocephargea. If patients with implante bone and under such as hepatitis. After thyroidbilirocytes spatem to phroot cause there is poin it is repaled to the Cardiagnosis is gimb-imple confect. Baral produce. Hope you are reason does notaly an anepsy postic. My suspendes on climine, and answed fluids, psychological cysts. Try kidney posi tek, burried infection infarction, least symptoms, and the environment of sepair dause level in the bed. You can go to a sore worried to the hands but less and consider fibroid sites, qi CTA?
```
## How to run the code

+ Install the requirements.
+ Download the validation and test data from the data folder.
+ For the train data, refer to the Medical GPT training data and use ```translate.ipynb``` to translate and get the training data
+ Upload the data files to your IDE.
+ Run the cells sequentially from the ```Promptologist.ipynb``` file.
