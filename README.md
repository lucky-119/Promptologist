# Promptologist
Large Language Model(LLM) for Medical Query Resolution

## 11-785 Introduction to Deep Learning Course Project
  + Aditi Patil (apatil2)
  + Aakriti Kinra (akinra)
  + Aryan Singhal (aryans)
  + Lakshay Arora (lakshaya)

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
```

## Description
Promptologist is the Course Project for our [11-785 Introduction to Deep Learning](https://deeplearning.cs.cmu.edu/F23/index.html#:~:text=the%20calendar%20first.-,OH%20Calendar,-%3A%20The%20Google) Course for Fall 2023.

## Goals
The goal of this project was to do do model distillation on a Large Language Model specifically in the field of medicine.

## Constraints

Our problem is specifically restrained to the field of Medical Consultation.

## Model Architecture

We tried a few models and picked the N-Gram model with Multi-Head Attention with Convolutional Layers as our best architecture

## Hardware

We trained the model on an NVIDIA Tesla T4 using Google Cloud Platform.

## Dataset

Our data includes English Patient-Doctor conversations and Chinese Patient-Doctor conversations converted to English.

## Data Preprocessing

+ Convert data from Chinese to English data using Google Translate.
+ Convert JSON Patient-Doctor conversations to line seperated texts.

## Evaluation Metrics

+ BERT Score
+ Cross-Entropy Loss

## Deliverables

+ [Midterm Report](https://www.overleaf.com/project/6555308f88f666a0c07a3fff)
+ [Final Report](https://www.overleaf.com/project/656cfe3aa78bbb74938b69a5)
+ [Project Video]()

## Samples
Input Prompt:
```
input prompt
```
Output:
```
output
```
