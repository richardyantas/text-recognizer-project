# Text recognizer project

Welcome!

Project developed during lab sessions of the [Full Stack Deep Learning Bootcamp](https://fullstackdeeplearning.com).

- We will build a handwriting recognition system from scratch, and deploy it as a web service.
- Uses Keras, but designed to be modular, hackable, and scalable
- Provides code for training models in parallel and store evaluation in Weights & Biases
- We will set up continuous integration system for our codebase, which will check functionality of code and evaluate the model about to be deployed.
- We will package up the prediction system as a REST API, deployable as a Docker container.
- We will deploy the prediction system as a serverless function to Amazon Lambda.
- Lastly, we will set up monitoring that alerts us when the incoming data distribution changes.

## Spring 2019 Bootcamp

  - Overview of the labs. 
  - Get set up. 
  - Lab 1 : Project structure. 
  - Lab 2 : Introduce EMNIST. Training code details. Train & evaluate character prediction baselines.
  - Lab 3 : Introduce EMNIST Lines. Overview of model architecture. Train our model on EMNIST Lines.
  - Lab 4 : Weights & Biases + parallel experiments.
  - Lab 5 : IAM Lines and experimentation time (launch a bunch of experiments, leave running overnight in a shared W&B). 
  - Lab 6 : line detection task
  - Lab 7 : data labeling
  - Lab 8 : continuous integration
  - Lab 9 : web deployment

# Setup

## 1. Sign up for W&B

- Go to https://app.wandb.ai
- Click 'sign up'
- Sign up with Github (or another if you prefer)
- Select whatever username you want

## 2. Setup a JupyterLab instance

- Go to https://app.wandb.ai/profile
- Enter the code we will share with you at the session into Access Code field.
- You should be dropped into a JuypyterLab instance with 2 GPUs to use for labs.

*From now on, do everything else in that instance*

## 3. Check out the repo

You should already have the repo in your home directory. Go into it and make sure you have the latest.

```sh
cd fsdl-text-recognizer-project
git pull origin master
```

If not, open a shell in your JupyterLab instance and run

```sh
git clone https://github.com/gradescope/fsdl-text-recognizer-project.git
cd fsdl-text-recognizer-project
```


## 4. Set up the Python environment

Run

```sh
pipenv install --dev
```

From now on, precede commands with `pipenv run` to make sure they use the correct
environment.

# Ready

Now you should be setup for the labs. The instructions for each lab are in readme files in their folders.

You will notice that there are solutions for all the labs right here in the repo, too.
If you get stuck, you are welcome to take a look!
