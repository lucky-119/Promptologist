# Promptologist
Large Language Model(LLM) for Medical Query Resolution

## 11-785 Intro to Deep Learning Course Project
  + Aditi Patil
  + Aakriti Kinra
  + Aryan Singhal
  + Lakshay Arora

## Description
Promptologist is the Course Project for our [11-785 Introduction to Deep Learning](https://deeplearning.cs.cmu.edu/F23/index.html#:~:text=the%20calendar%20first.-,OH%20Calendar,-%3A%20The%20Google) Course for Fall 2023

## Goals
The goal of this project was to do do model distillation on a Large Language Model specifically in the field of medicine.

## Constraints

Our problem is specifically restrained to the field of Medical Consultation.

## Model Architecture

We tried a few models and picked the N-Gram model with Multi-Head Attention as our best architecture.
###to update###

## Hardware

We trained the model on an NVIDIA Tesla T4

## Dataset

Our data includes English Patient-Doctor conversations and Chinese Patient-Doctor conversations converted to English.

## Data Preprocessing

+ Convert Chinese data into English data using Google Translate.
+ Convert json Patient-Doctor conversations to line seperated texts.

## Evaluation Metrics

+ BERT Score
+ Cross-Entropy Loss
