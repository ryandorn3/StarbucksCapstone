# Starbuck's Capstone Project
### Installations:
- import pandas as pd
- import numpy as np
- import math
- import json
- import sqlite3
- import matplotlib.pyplot as plt
- % matplotlib inline
### Project Motivation:
For this analysis we want to determine which customers have a higher conversion rate when an offer is presented, along with total non offer transactions. We will be looking at customer breakdowns by age, gender, member year, and income. This will allow us to better understand which customers we should be sending offers to and those who we should not.
### Files Used:
1. portfolio.json
  - id (string) - offer id
  - offer_type (string) - type of offer ie BOGO, discount, informational
  - difficulty (int) - minimum required spend to complete an offer
  - reward (int) - reward given for completing an offer
  - duration (int) - time for offer to be open, in days
  - channels (list of strings)

2. profile.json
  - age (int) - age of the customer 
  - became_member_on (int) - date when customer created an app account
  - gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
  - id (str) - customer id
  - income (float) - customer's income

3. transcript.json
  - event (str) - record description (ie transaction, offer received, offer viewed, etc.)
  - person (str) - customer id
  - time (int) - time in hours since start of test. The data begins at time t=0
  - value - (dict of strings) - either an offer id or transaction amount depending on the record
### Acknowledgements:
- The datsets were provided by Starbucks
