# Welcome to Algolia's ML technical challenge.

## The Challenge

We want to predict the most likely user to answer a question, given its title & text. We'll work with a public Stack Overflow dataset. Using additional data besides the one provided is not allowed, but you can use pre-trained models if needed. 

You can download the data [here](https://drive.google.com/file/d/1CUcfl3JX8TNYABn2JRIPQozT0oqdqqOy/view?usp=sharing).

We provide 3 dataset files: users.json, questions.json, answers.json in JSON newline delimited format. A question can have multiple answers, sent by different users. A question is considered resolved if it contains an `accepted_answer_id`, linking to the accepted response from the answers dataset. 

For this problem, we're looking to provide a **list of potential users that can answer a question**, but the answer doesn't have to be accepted.

The result will be a CSV or JSON of the form: question_id,user1_id,...,user20_id. The users should be ranked in descending order from the most probable to the least probable to answer the question. Indeed, we only want to predict up to 20 relevant users. From the questions dataset, you can choose a subset of random questions for which to provide these results.

## What you need to return

At the end of the challenge, please share the solution in the form of a reproductible notebook (i.e. Runtime -> Run all cells -> CSV exported) or Python script.

Please also provide a description of your solution in the notebook (markdown format) or script, as well as a short analysis of your results and potential improvements.

## The evalution

You will be evaluated on the following points:
* Overall approach and steps taken to solve the problem 
* Quality of your code (time and memory complexity, comments, naming convention, typing, ...)
* Your analysis and potential improvements

Good luck, and do not hesitate contacting us if you have a question!
