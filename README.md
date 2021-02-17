# ML-challenge

Welcome to Algolia's technical challenge.

What we want to do here is to predict the most likely user to answer a question, given its title & text. We'll work with a public dataset, however using additional data besides the one provided is not allowed. At the end of the challenge, each participant must share the solution in the form of a reproductible notebook (i.e. Runtime -> Run all cells -> CSV exported).

You can download the data <a href="https://drive.google.com/file/d/1ysfkiUMeDI5FmvIHKd-J40PQgN51Zb-N/view?usp=sharing">here</a>.

We provide 4 dataset files: <em>users.csv, questions_train.csv, answers_train.csv, questions_test.csv</em>. In the training file we have a set of questions and provided answers. Each question has been marked as resolved by the user using one of the answers offered by the other users.

The challenge here is, for the test questions, to provide a list of potential users ranked in descending order from the most probable to the least probable, that might answer this question. We know for a fact that each question has been already answered by one of the users.

The result will be a CSV of the form: `question_id,user1_id,...,user20_id`.Indeed, we only want to predict up to 20M relevant users. The computed metrics will be Precision@K=1, K=5 and K=20 as well as Mean Reciprocal Rank.