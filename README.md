# Artificial Digital Agent Assignment

## Challenge:

Build a model using any tooling that you feel is right (LLM, GPT, BERT, NLP) and fine-tune it on based on the `dataset` folder where there are two documents:
1. knowledge-base.md
2. conversations.json

The Agent will not be trained based on `live-datasource.json` But the agent can use this as live data during runtime.

## Objective

Develop a conversational language model (LLM) tailored for a business environment, focusing on providing general support, managing new account openings, blocking credit cards, and advising on investments, loans, and insurance. The model will be trained using knowledge base and conversations as unsupervised learning methods. The digital agent can query live through `live-datasource.json` file and provide answers to customer questions.

IMPORTANT NOTE: Do not use third-party AI API such as OpenAI ChatGPT for this test, we wish to see how you fine-tune a model.

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

We will replace in our end the `live-datasource.json`, `knowledge-base.md`, `conversions.json`.
Which will include new rules and new conversations and data source. in this change structure of live-datasource
and conversations will remain the same, just a larger dataset will be used to test effectiveness of your solutions.

To give you some hints:
- The test is to see how do you apply Supervised, Semisupervised or Unsupervised training.
- How do you create test for your solution.
- How to ensure your user data privacy.
