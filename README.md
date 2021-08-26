# Welcome to Algolia's ML technical challenge.

## The Challenge

What we want to do here is to predict the most likely user to answer a question, given its title & text. We'll work with a public dataset, however using additional data besides the one provided is not allowed. 

You can download the data [here](https://drive.google.com/file/d/1ysfkiUMeDI5FmvIHKd-J40PQgN51Zb-N/view?usp=sharing).

We provide 4 dataset files: users.csv, questions_train.csv, answers_train.csv, questions_test.csv. In the training file we have a set of questions and provided answers. Each question has been marked as resolved by the user using one of the answers offered by the other users.

The challenge here is, for the test questions, to provide a list of potential users ranked in descending order from the most probable to the least probable, that might answer this question. We know for a fact that each question has been already answered by one of the users.

Since there is a lot of data, we recommend you start with a subsample that your machine can manage and extend to the full dataset when your method is ready.

The result will be a CSV of the form: question_id,user1_id,...,user20_id.Indeed, we only want to predict up to 20M relevant users. The computed metrics will be Precision@K=1, K=5 and K=20 as well as Mean Reciprocal Rank.

## What you need to return

At the end of the challenge, each participant must share the solution in the form of a reproductible notebook (i.e. Runtime -> Run all cells -> CSV exported), as well as the following metrics on the test data.
* Precision@K=1, K=5, and K=20
* Mean Reciprocal Rank

Please also provide a description of your solution in the notebook (markdown format) as well as an analysis and a discussion of your results, and potential improvements.

## The evalution

You will be evaluated on the following point:
* Quality of your solution
* Quality of your code (time and memory complexity, comments, naming convention, typing, ...)
* Your analysis and potential improvements

Good luck, and do not hesitate contacting us if you have a question!
