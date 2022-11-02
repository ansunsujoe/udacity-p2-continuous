# udacity-p2-continuous-control

In this project, we will be training a DDPG agent to move a double-jointed arm to target locations.

## Project Details

This task is single-agent and episodic and has a continuous action space. The high-level goal is to guide an arm to target locations in a space.

**State Space**: contains 33 dimensions and contains the agent's arm's position, rotation, velocity, and angular velocities.

**Action Space**: A continuous vector with 4 dimension (torque for each of the joints).

**Rewards**: We will get a reward of +0.1 for each step that the agent's hand is in the goal location.

**Goal**: In order to solve the environment, our agent must get an average score of +30 over 100 consecutive episodes.

## Getting Started

**Step 1:** Clone the Udacity deep-reinforcement-learning project.

```
git clone https://github.com/udacity/deep-reinforcement-learning.git
```

**Step 2:** Copy the folder called "python" in the Udacity deep-reinforcement-learning project into the root directory of this project. This contains the code required to run a Unity environment.

**Step 3**: Open the Jupyter notebook "Control.ipynb" and run the first cell in Step 1 in order to install all the necessary Python packages and the unityagents package.

## Instructions

Here are the steps that are required in order for you to be able to train a DDPG agent on the Reacher environment.

**Step 1:** Run all the cells in sections 1-7 of Control.ipynb. This will set up all the classes and functions needed for training a DDPG.

**Step 2:** At the beginning of section 8 of the notebook, replace the file path of the Reacher Environment with the file path for your executable.

```
# Create environment
env = ReacherEnvironment(fp="/your-file-path")
```

**Step 3:** Tweak any hyperparameters that you want in the initialization of the agent or the calling of the train_ddpg method in Section 8.

**Step 4:** Run the code cell in section 8 and watch your DDPG being trained!