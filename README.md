# Multi-Armed-Bandits
Multi-Stage-Multi-Armed Bandits (MAB) are a class of reinforcement learning problems where an agent tries to maximize its cumulative reward by sequentially selecting actions from multiple options (arms) and observing the rewards associated with those actions.

In a Multi-Stage Multi-Armed Bandits model, the environment or the problem faced by the agent evolves over multiple stages or time periods. At each stage, the agent selects an action (arm) based on its current knowledge or belief about the rewards associated with each action. As the agent interacts with the environment, it learns more about the rewards of each action and can adapt its strategy accordingly.

These models are particularly useful in dynamic decision-making problems where the underlying parameters or conditions change over time. They find applications in various fields such as online advertising, clinical trials, resource allocation, and network routing, among others.

## Model Stages:

# stage 1 - building agent arms

building an Arm: theory development In the initial phase, upon evaluating the idea’s feasibility and pragmatism for a theory, the DM determines the number of arms to develop within her operational constraints. This step establishes the groundwork for the problem. Subsequently, she enters a pure exploration phase, conducting experiments to evaluate the arms. The final stage then navigates the dynamics of exploration versus exploitation in the investment.

# stage 2 - test agent arms

Best arm identification: experimentation
In this stage the goal of DM is not choosing the best arm, while it’s a pure exploration experimentation stage where she tries run experiments and collect information toward updating the expected value of arms and to identify the best arm among a set of k arms.

# stage 3 - invest agent arms

Selecting an Arm: Investment decision In this stage after the experimentation, it is the time for DM to select an arm and invest on it. and observe a real reward. Reward at this stage has 2 signals on both profit and the V (which is the probability of state of interest) so observation of rewards will update the prior of both. Since in this stage is highly costly so we introduce a switching cost based on Manjari and Teneketzis (1996) and where they argued in every time the processor switches from one machine to another, a switching cost (which can be the cost of switching or switching delay) is incurred. The inclusion of switching cost is a realistic consideration for our setup because in the case of LFHI decisions it needs a huge amount of investment to select an arm and run it. Thus, when DM finds a better opportunity which has higher expected profit as reward in this stage she faces a high cost of switching or delay in switching.

# Problem Solution:

* The solution method focuses on minimizing loss and making optimal investment decisions.
* Endogenously determined arms are developed within defined constraints.
* BAI is used to rank theories and facilitate effective experiments.
* Consideration of switching costs and budgetary constraints is crucial for optimizing investments.
* Killing the arm strategy is employed to remove arms with low expected value, reducing waste in cognitive and resource resources.
