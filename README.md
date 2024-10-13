# Question Answering System for Stunting Information

This repository contains the code for a thesis project titled "QUESTIONS ANSWERING SYSTEM FOR A STUNTING INFORMATION SERVICE BASED ON OPEN SOURCE LANGUAGE MODELS". The project compares the performance of a Retrieval-Augmented Generation (RAG) based question answering system and a retrieval-based question answering system on the topic of stunting using open-source Large Language Models (LLMs).

## Overview
Large Language Models (LLMs) can provide information based on data they were trained on, but they have limitations when it comes to retrieving the most up-to-date information, such as recent developments in stunting. To address this, the system adopts a Retrieval-Augmented Generation (RAG) approach, where it retrieves data from external sources, specifically the Cegah Stunting website.
The goal is to evaluate which approach performs better in answering stunting-related questions: RAG or traditional retrieval-based systems.

## Features
### Two RAG Systems: 
Built using the LangChain framework, the project implements two types of RAG systems:
- Retrieval QA Chain
- Conversational Retrieval Chain with memory support

### Open-Source Language Models:
- Flan-T5 small
- Flan-T5 base
- Flan-T5 large

### Baseline Comparison: 
The project also includes a Retrieval-Based Question Answering System (without LLMs) for performance comparison.

## Data Source
The external data used by the RAG systems is pulled from the Cegah Stunting website.

## Evaluation
The system is evaluated using 15 question-answer pairs that are categorized into:
- Independent questions: Stand-alone questions with no relation to previous ones.
- Related questions: A sequence of related questions that form a chain.

## How to Replicate
### Run the Question Answering System Stunting code:
- Start by installing all the necessary libraries.
- Then, proceed to crawl and scrape data from relevant sources.
- Process the retrieved data by performing preprocessing.
- Save the processed documents in JSON format.

### Run evaluation code:
- After saving the documents, open the evaluation section in the notebook.
- There are two types of evaluations that can be conducted: related questions and independent questions.
- To perform the evaluation, run all the steps from the beginning to the end.
- In the Load Dataset QA section, input the Excel file containing 15 question-answer pairs.
