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

This project will create a model that can detect noise sources in audio. The model will be trained on voice samples combined with a variety of noise sources
(air conditioner, vehicles, etc.) from Microsoft's Scalable Noisy Speech Dataset, and return whether or not the original source is noisy. The project will be
deemed succesful if it is fairly accurate (significantly above the base rate of 50%). This project is a scaled down version of a full denoiser, and thus is 
useful for the creation of clean audio that can be used in music or further analysis.

<!-- What problem your project addresses.
The overall approach you will use to solve the problem.
How you propose to evaluate your success against your stated goals. -->

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

Charlie:
I am very excited to begin working with audio files. My goals were mainly around contributing equally to all areas of the project, from proposal to creation to presentation, and I plan on doing so to learn as much as I can about how the complete machine learning pipeline works with respect to audio. Specifically, I am excited about learning how audio files are encoded and the process of vectorizing them for our model. Also, I want to learn how to publish an open-source python package so that our project can be used by others in the future.
Lastly, I also had a goal to communicate well with my group, and I want to use it as an opportunity to solidify my git workflow with respect to working in feature branches and creating pull requests for Jeff to review.

## Risk Statement - Jeff

What are two things that could potentially stop you from achieving the full deliverable above? Maybe it turns out that the pattern you thought would be present in the data just doesn’t exist? Or maybe your idea requires more computational power than is available to you? What particular risks might be applicable for your project?

- computational power

## Ethics Statement

Who benefits from this project?
This project will benefit the audio community. The ability to identify noise in audio files will allow us to then clean them up and remove the excess noise. This could be useful for anyone from musicians to podcasters to filmmakers - people who need to record audio and want to make sure it's as clean as possible so that the audience can hear it clearly and have a better listening experience.

Who has the potential to be excluded from benefit or even harmed from this project?
Our data includes spoken audio by male and female speakers. However, English is the only language used in the dataset, meaning our model will only be trained in English. This will exclude non-English speakers from potential benefits of the project, which is around 80% of the world's population.

Will the world become an overall better place because of this project? 
We think this project will help the world become a better place. Since denoising audio is the ultimately goal where this project will have the most impact, it will allow for clearer audio in the future - this will benefit everyone, especially those hard of hearing or people trying to translate a foreign language. The assumptions here are that this will help people communicate more effectively, and that training the model in English will still contribute to some level of increasing translation accuracy from audio.

## Tentative Timeline

After week three, we plan to have designed and completed our data collection. We also plan to have vectorized our data and begun the modeling process, showing some exploratory analysis.
By week six, we plan to have engineered our features and designed our model, and completed a full assessment of our model. And hopefully it works! :)