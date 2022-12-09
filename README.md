# Model Performance improvement methods
## Model-centric Approach
### Magnitude-based pruning
Magnitude-based pruning sets a threshold and drops weights below it in every training iteration. Those small weights have less contribution to the output and can be replaced by adjacent neurons and connections. By several training and pruning iterations, the network can be much smaller with the nearly same performance against the same training dataset. However, in this lab we cannot deploy this technique to the model due to the time-consuming training phase and limited resources. 
### Weight quantization and approximation
We can reduce the data precision by mapping weights to discrete levels, e.g., 1.01, 1.02, 0.99 are set to 1. Using this technique the model can use low bit-width data representation and as a result we can reduce the area and energy cost of the model. 
## Data-centric Approach
In the inference UI, users can paste a YouTube URL to transcribe the video. We think those videos are well-labeled (accurate subtitles) and we can use those data to train our model. With more users and data, we can train a better model which will bring us more users and data.

### Training Results





# Deployment

https://huggingface.co/spaces/qisan/whisper-small-CN-YouTube-video-transcribe

![Alt text](https://github.com/Chaouo/Titanic_serverless_ML/blob/main/data/Screenshot 2022-12-09 at 13.39.03.png)

