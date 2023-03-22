# CS-4403-Assignment-3

# The Task:

A local bank has come to our class for help. They have been lending out money to a large community for decades, but are unhappy with how good they are in deciding to lend money to the right people. They would like greater insight into what it is about their customers that influences whether loans get paid back or not.

They have provided us with a good size dataset spanning many years of lending activity.

The dataset contains the following data for over 7700 past loans:

- default: 1 for a default on the loan, 0 for paid back in full.
- amount_of_loan: how much was lent out.
- credit_rating: from A to G. A is great, G is not so great.
- years_with_bank: how long the customer has been with the bank.
- rent_mortgage_own: 0 for own, 1 for mortgage, and 2 for owner (without any debt).
- income: the annual income of the customer at the time of the loan.
- age: the age of the customer at the time of the loan.

The dataset as a CSV can be found here.

(the dataset does require a little bit of cleanup and transformation, but nothing that you cannot now easily handle :)

The goal for this assignment is to find an optimal model for predicting a new loan applicant's likelihood of paying back a new loan.

Use any algorithm to build a classification model for this dataset, subject to the following constraints:

- you should split the dataset into a training and test set, with a test set of at least 20%.

- you must use at least two of the six features.

- The key metric will be Accuracy, with an emphasis on keeping false positives low, and in any event lower than any false negatives (the bank has told us that they do not want to refuse a loan for someone who would have paid it back, but would rather not lend to someone who was predicted as not defaulting, when they will). 

- Your model should be cross-validated.

You should feel free to use ensemble versions of algorithms (where available), as well as Grid Search to find optimal hyperparameters. You will want to try all of the algorithms we have studied so far.
