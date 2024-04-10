# CS0451_Denoising

DETECTING NOISE:

https://github.com/microsoft/MS-SNSD


Original Warmup Proposal:

This project will address noise levels in audio recordings. Particularly, it will identify the presence of noise as a first step toward denoising audio signals.
There is a noisy speech corpus called MS-SNDS (https://github.com/microsoft/MS-SNSD) that is perfect for this project. It provides human voices with different levels and types of noisiness, as well as the clean versions of these signals.
This is a classification problem, as the machine would determine whether or not a voice signal is noisy. I think the next step (denoising these signals/outputting the clean signal version) would be outside the scope/timeframe of this class.
I would judge this project to be successful if the model can accurately predict if a signal has noise inserted into the audio file. In particular, similar accuracy rates across the different noise sources the database provides would be ideal.
I’m an electronic musician who often works in lofi production setups. These setups often end up creating a lot of artifacts due to a lack of audio treatment, background noise, etc. Identifying noise sources in audio is the first step to creating an algorithm that accurately denoises audio sources.


________________________________________________________________________________________________


## Abstract - Jeff

In 3-4 sentences, concisely describe:
What problem your project addresses.
The overall approach you will use to solve the problem.
How you propose to evaluate your success against your stated goals.

## Motivation and Question - Jeff

Describe your motivation for your project idea. Some (shortened) examples of good types of motivations:
We have a scientific data set for which predictive or exploratory models would help us generate hypotheses.
We have user information for which predictive models would help us give users better experiences.
We have performance data (e.g. from sports teams) for which predictive models could help us make better decisions.
Algorithmic bias is an increasingly urgent challenge as machine learning products proliferate, and we want to explore it more deeply.
You should be more specific than these: describe your specific data set (if applicable); your scientific questions; the type of decisions your model could inform; etc.

- clean audio is GOOD

## Planned Deliverables

We have two planned deliverables:
1) A python package that effectively classifies an audio file as either clean or noisy. This package will contain our full documented machine learning pipeline.
2) A Jupyter notebook that demonstrates the use of our package to classify audio files as clean or noisy.

"Full success" for us is detecting the presence of noise in audio files with high accuracy. 
"Partial success" would be only detecting the difference between a clean audio file and a file that is only noise. Since our data consists of A) clean audio files and B) types of background noise, we will have the pure noise files to compare against the clean ones. This would indicate that we have made progress and are well on our way, but weren't able to make our final model accurate enough.

## Resources Required - Jeff

What resources do you need in order to complete your project? Data? Computing power? An account with a specific service?
Please pay special attention to the question of data. If your project idea involves data, include at least one link to a data set you can use. If you can’t find data for your original idea, that’s ok! Think of something related to your group’s interests for which you can find data.
Most projects should involve data in some way, but certain projects may not require data. Ask me if you’re not sure.

- access to ada for parsing through thousands of .wav files
- scikit audiolab for dealing with audio files

## What You Will Learn - Both

Each group member should return to their stated goals from the reflective goal-setting assignment at the beginning of the course. Then, in this section, please state what each group member intends to learn through working on the project, relating your intentions to your stated goals. You might be thinking of certain algorithms, software packages, version control, project management, effective teamwork, etc.

## Risk Statement - Jeff

What are two things that could potentially stop you from achieving the full deliverable above? Maybe it turns out that the pattern you thought would be present in the data just doesn’t exist? Or maybe your idea requires more computational power than is available to you? What particular risks might be applicable for your project?

- computational power

## Ethics Statement - Charlie

All projects we undertake involve decisions about whose interests matter; which problems are important; and which tradeoffs are considered acceptable. Take some time to reflect on the potential impacts of your project on its prospective users and the broader world. Address the following questions:
What groups of people have the potential to benefit from our project?
What groups of people have the potential to be excluded from benefit or even harmed from our project?
Will the world become an overall better place because we made our project? Describe at least 2 assumptions behind your answer. For example, if your project aims to make it easier to predict crime, your assumptions might include:
Criminal activity is predictable based on other features of a person or location.
The world is a better place when police are able to perform their roles more efficiently.
If your project involves making decisions or recommendations, then you will also need to consider possible forms of algorithmic bias in your work. Here are some relevant examples:
A recipe recommendation app can privilege the cuisines of some locales over others. Will your user search recipes by ingredients? Peanut butter and tomato might seem an odd combination in the context of European cuisine, but is common in many traditional dishes of the African diaspora. A similar set of questions applies to recommendation systems related to style or beauty.
A sentiment analyzer must be trained on specific languages. What languages will be included? Will diverse dialects be included, or only the “standard” version of the target language? Who would be excluded by such a choice, and how will you communicate about your limitations?

- benefits audio community. anyone recording
- probably won't harm anyone, but none English speakers would be at a disadvantage since it is trained on English words. (excluded from benefit)

- we think it will help the world become a better place! Especially where clearing up audio is concerned, we think it'll at least contribute to more explicit audio translation, which will help the world come together :) <3 

## Tentative Timeline

After week three, we plan to have designed and completed our data collection. We also plan to have vectorized our data and begun the modeling process, showing some exploratory analysis.
By week six, we plan to have engineered our features and designed our model, and completed a full assessment of our model. And hopefully it works! :)