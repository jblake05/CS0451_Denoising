# CS0451_Denoising

https://github.com/microsoft/MS-SNSD

## Abstract - Jeff

This project will create a model that can detect noise sources in audio. The model will be trained on voice samples combined with a variety of noise sources
(air conditioner, vehicles, etc.) from Microsoft's Scalable Noisy Speech Dataset, and return whether or not the original source is noisy. The project will be
deemed succesful if it is fairly accurate (significantly above the base rate of 50%). This project is a scaled down version of a full denoiser, and thus is 
useful for the creation of clean audio that can be used in music or further analysis.

## Motivation and Question - Jeff

Our motivation behind this project comes from our access to the MS-SNSD (speech dataset, mentioned above) which could help in the algorithmic denoising of audio sources.
As electronic musicians, achieving a noise-free or noise-reduced audio sample is difficult to achieve on a low budget -- acoustic treatment and a studio environment is typically
needed for a more professional sound. Cleaner audio is also helpful for different audio analysis tasks, such as models that automate subtitles or translation. Thus, this project
will create a model that can be useful for musicians and further audio programming work. One question going into this project involves exploring how vectorization of audio files
could work in a way that is efficient and scalable across a large dataset.

## Planned Deliverables - Charlie

We have two planned deliverables:
1) A python package that effectively classifies an audio file as either clean or noisy. This package will contain our full documented machine learning pipeline.
2) A Jupyter notebook that demonstrates the use of our package to classify audio files as clean or noisy.

"Full success" for us is detecting the presence of noise in audio files with high accuracy. 
"Partial success" would be only detecting the difference between a clean audio file and a file that is only noise. Since our data consists of A) clean audio files and B) types of background noise, we will have the pure noise files to compare against the clean ones. This would indicate that we have made progress and are well on our way, but weren't able to make our final model accurate enough.

## Resources Required - Jeff

We'll likely need access to ada to complete this project, both for its storage space and its computational power (since we'll be parsing through thousands of wave files). We also need access to a dataset of voice and noise sources, but this is provided in https://github.com/microsoft/MS-SNSD. This dataset has thousands of clean voice sources alongside around one hundred different noise sources, so we'll use it to generate the training and testing data through combination.

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