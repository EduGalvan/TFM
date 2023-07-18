# Design and study of an open-ended questionnaire on anxiety
Use of data augmentation techniques with generative AI, aswell as textual analysisi of the generated data.

In this project for my Master´s thesis we try to create an validate an open ended response questionnarie on anxiety. Because the process of data gathering was nearly impossible we decided to use data augmentationt techniques, and in this context, for this particula problem i tried to use a LLM to create synthetic data from the originial responses to our questionnarnaire which only 15 people ended up answering.

We use the chatGPT-API and with recursive calls with a specific prompt for each knwoledge category ended up with a database of around 100 individuals an 600 total ansewrs.

Later we used this generated dataframe to train a model to predcit the categorie of knowledge each ansewr was on based on the text of the answer, for this we used a LSTM network to work with the processed data.

We ended up yielding good resutswith the rig hyperparameters tuning, of around a 77% accuracy across all of the Items. This results may have been much better if we had more quality samples to create the prompts with.
