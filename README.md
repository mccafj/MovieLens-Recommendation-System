# MovieLens Recommendation System

Authors: Samuel Robins, Jon McCaffrey

Build a model that provides top 5 movie recommendations to a user, based on their ratings of other movies.

You will need to create the specific details about how the user will provide their ratings of other movies, in addition to formulating a more specific business problem within the general context of "recommending movies".

At minimum, your recommendation system must use collaborative filtering. If you have time, consider implementing a hybrid approach, e.g. using collaborative filtering as the primary mechanism, but using content-based filtering to address the cold start problem Links to an external site..

The MovieLens dataset has explicit ratings, so achieving some sort of evaluation of your model is simple enough. But you should give some thought to the question of metrics. Since the rankings are ordinal, we know we can treat this like a regression problem. But when it comes to regression metrics there are several choices: RMSE, MAE, etc.

Overview / initial summary (~250 wds)
- business / data understanding - what kind of data are you using?  and what makes it well-suited for the business problem
- data prep - why did you choose the data prep steps that you did?  and what was the result
- modeling - what modeling packages did you use, which models within the packages, and what tuning steps did you take?
- evaluation - How well did your model perform?  Relevant metrics.  Validation approach


Business and Data Understanding


Data preparation: feature engineering, using pipelines or using unsupervised techniques


Modeling: rationale, results, limitations, and recommendations
- using models from multiple different packages or model explainability tools

Rationale

Results

Limitations / recommendations

Evaluation (ending summary)

For More Information
Please review our full analysis in our Jupyter Notebook or our presentation.

For any additional questions, please contact Andrew Boucher aboucher1360@gmail.com or Jon McCaffrey jonmccaffrey524@gmail.com

Repository Structure

├── README.md
├──  .ipynb  <- Main notebook for project code
├──  slides.pdf      <- PDF of slides for our presentation
├── Data			                          <- Location of raw dataset
└── Images                              <- images used and generated in the project
