# Image Classification using AWS SageMaker

Use AWS Sagemaker to train a pretrained model that can perform image classification by using the Sagemaker profiling, debugger, hyperparameter tuning and other good ML engineering practices. This can be done on either the provided dog breed classication data set or one of your choice.

## Project Set Up and Installation
Enter AWS through the gateway in the course and open SageMaker Studio. 
Download the starter files.
Download/Make the dataset available. 

## Dataset
The provided dataset is the dogbreed classification dataset which can be found in the classroom.
The project is designed to be dataset independent so if there is a dataset that is more interesting or relevant to your work, you are welcome to use it to complete the project.

### Access
Upload the data to an S3 bucket through the AWS Gateway so that SageMaker has access to the data. 

## Hyperparameter Tuning
The model I used for this project was ResNet50 as it  has demonstrated excellent performance on various computer vision tasks, such as image classification and object detection. Its deep architecture, with 50 layers, enables it to learn complex representations and capture intricate patterns in the data, leading to accurate and reliable predictions.
The hyperparameter's I tuned are Learning rate and Batch size. Choosing an appropriate learning rate is crucial for successful model convergence. If the learning rate is too high, the model may fail to converge, leading to unstable or poor performance. The choice of batch size can impact both the computational efficiency and the quality of the learned model. The ranges I provided and used are as follows: 
"lr": ContinuousParameter(0.001, 0.1),
"batch-size": CategoricalParameter([20, 34, 40, 60, 75]).
![Completed Hyperparameter Tuning Jobs](hpy_jobs.png)

Remember that your README should:
- Include a screenshot of completed training jobs
- Logs metrics during the training process
- Tune at least two hyperparameters
- Retrieve the best best hyperparameters from all your training jobs

## Debugging and Profiling
**TODO**: Give an overview of how you performed model debugging and profiling in Sagemaker

### Results
**TODO**: What are the results/insights did you get by profiling/debugging your model?

**TODO** Remember to provide the profiler html/pdf file in your submission.


## Model Deployment
**TODO**: Give an overview of the deployed model and instructions on how to query the endpoint with a sample input.

**TODO** Remember to provide a screenshot of the deployed active endpoint in Sagemaker.

## Standout Suggestions
**TODO (Optional):** This is where you can provide information about any standout suggestions that you have attempted.
