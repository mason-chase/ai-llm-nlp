# ai-llm-nlp

# Task: Sentiment Analysis with Language Models

## Challenge:

Build a sentiment analysis model using a pre-trained LLM (e.g., GPT, BERT) and fine-tune it on based on the `dataset` folder where there are two documents:
1. knowledge-base.md
2. conversations.json

The Agent will not be trained based on `live-datasource.json` But the agent can use this as live data during runtime.

## Objective

Develop a conversational language model (LLM) tailored for a business environment, focusing on providing general support, managing new account openings, blocking credit cards, and advising on investments, loans, and insurance. The model will be trained using a combination of supervised and unsupervised learning methods, with business documents serving as the foundation for unsupervised training, and a curated Q&A list for supervised training. The agent is able to query in live through `live-datasource.json` file and provide answers to customer questions.

## Bonus

Experiment with different LLMs (e.g., GPT, BERT, XLNet) and compare their performance.
Implement techniques for handling imbalanced datasets if applicable.
Explore techniques like data augmentation or adversarial training to improve the model's robustness.

## Delivery and Testing

- You will receive a Virtual Machine with a limited time of 24 hours at maximum to train your model.
- Your solution must be tested base and having Unit Tests to that would explain the logic and acceptance criteria
- Your model must have an interface of a test base chat model
- We can replace the files in `dataset` folder with new data retrain your model live together and test the result.
  
## Test Conversation Result

Your agent should be able to ask a question if the user's request is not in full detail.

Example:
```
Customer: Hi, I wish to request charge back
Agent: May I know the date, amount and merchant name?
Customer: The amount is 198.20 and date is: "10-OCT-2022" from 
Agent: I have found this transaction and it is not qualified for chargeback, is there other transaction I can help you with
Customer: Yes, amount is amount 7849.90 from LG on December 12
```