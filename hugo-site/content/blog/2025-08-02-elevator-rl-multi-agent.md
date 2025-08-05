---
title: Elevator RL Multi-Agent
date: 2025-08-02T10:00:00+09:00
draft: false
slug: elevator-rl-multi-agent
---
<!-- Note: To display the image, please save it to hugo-site/static/images/ folder and uncomment the line below -->
<!-- ![Elevator RL Multi-Agent Screenshot](/images/elevator-rl-multi-agent-screenshot.jpg) -->

## Why
- In order to gain an understanding of more complex RL algorithms working with the FlexSim model, which includes state machine logic, multi-agent passenger management, and complex observation spaces

## How
- Read and understood how the learning algorithm interfaced with the FlexSim via the state machine diagrams
- Read about how the system uses action masking (A vector to store decisions) to output decisions to act upon
- Ran the corresponding Python files to see it in action (The environment, the training, and the inference based on the trained model)
- Learned about command `tensorboard --logdir=.` in order to see the Tensorboard interface, and model results without using the command palette interface
- Notice the difference in performance of the FlexSim model with the trained RL model making decisions rather than taking random decisions

## So What
- Completing and understanding this allows for the bridging with previous more simpler concepts (From HelloWorld) to more complex agent models to understand in the future

[Original Notion page](https://grave-flood-782.notion.site/Elevator-RL-Multi-Agent-8-2-2426575c333a80e8a5cbdba481b418a8)