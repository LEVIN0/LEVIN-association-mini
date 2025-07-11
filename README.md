# levin-association-mini
-This repository contains a Python script for simulating transactional data and analyzing it using the Apriori algorithm to uncover  car-shopping patterns.

## Objective
Simulate basic car shopping transactions and use the Apriori algorithm to discover associations between items.
-<img width="990" height="688" alt="image" src="https://github.com/user-attachments/assets/4973bdc4-500f-4738-94d7-f0b7f270e16b" />
- l imported the necessary packages to perform this task and then generated 10 transactions  of cars and then l was able to display the 10 transactions after ensuring they are picked at random in the set.seed and then ensured no duplicates were there
- <img width="817" height="605" alt="image" src="https://github.com/user-attachments/assets/23d4f0be-3bce-4588-99b5-966dae8e3bd9" />
- l then changed the data into a one-hot encoded format
- This is done so that the transactional data can be changed into binary format to allow the Apriori algorithm to count combinations of items in a structure it can understand
- <img width="729" height="481" alt="image" src="https://github.com/user-attachments/assets/ad2820eb-5d95-4090-afb8-1ef5ed04cb98" />
- l then used Apriori algorithm to find the most frequent item-sets with a support of >=0.3
- support is the measure of how frequently an item or itemset appears in the entire dataset of transactions.
- Isuzu has the highest support from the data shown
-<img width="894" height="359" alt="image" src="https://github.com/user-attachments/assets/bb0ded05-c2d6-4e52-bdaa-c01c9c2c8566" />
- l used the rule of confidence of a threshold of 0.7 
- the confidence rule shows what are the chances for car B being bought if car A has been bought

## Sample Rule
- <img width="1493" height="353" alt="image" src="https://github.com/user-attachments/assets/32d9423a-212d-42a7-bbfa-5de2c22d64ec" />
**If a customer buys Merc , they are likely to buy Isuzu (100% confidence)**

## What it means:
In real life, it suggests these items are often bought together. Retailers could use this insight for marketing or stock replacement.

## How to Run
- Install required packages: `pip install pandas mlxtend`
- Run `association_rules_mini.py` or open `notebook.ipynb`
