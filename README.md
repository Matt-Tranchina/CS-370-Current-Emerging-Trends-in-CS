# Pirate Treasure Hunt Game
This is a treasure hunting game where the player (user) versus a pirate (an intillegent agent) in a race to traverse a maze to find and capture the treasure. The goal of this game is to traverse a maze and reach the treasure before the pirate does. The goal of this project is to design the intelligent agent as an NPC (non-player character) to represent the pirate which will navigate the game world that consists of different pathways and obstacles, in order to find the treasure before the human user does. 
## Code given vs Code created
This project is built using Python as well as the TensorFlow and Keras libraries.\
**The enviornment** for the agent has already been designed as a maze (8X8 matrix), containing free (1), occupied (0), and target (1 at the bottom right) cells, as below:

 [ 1., 0., 1., 1., 1., 1., 1., 1.],\
 [ 1., 0., 1., 1., 1., 0., 1., 1.],\
 [ 1., 1., 1., 1., 0., 1., 0., 1.],\
 [ 1., 1., 1., 0., 1., 1., 1., 1.],\
 [ 1., 1., 0., 1., 1., 1., 1., 1.],\
 [ 1., 1., 1., 0., 1., 0., 0., 0.],\
 [ 1., 1., 1., 0., 1., 1., 1., 1.],\
 [ 1., 1., 1., 1., 0., 1., 1., 1.]

 The agent starts at the top left and can move in four directions: Left, Right, Up, and Down.\
 The **TreasureEnviornment.py** has been provided and contains complete code for the enviornment, including the maze object mentioned above as well as code that supports methods for resetting the pirate position, updating the state based on pirate movement, returning rewards based on agent movement guidelines, keeping track of the state and total reward based on agent action, determining the current enviornment state and game status, listing actions from the current cell, and a visualization method for graphical display of enviornment and agent action.\
 
 The **GameExperience.py** was also provided and contains complete code for experience replay. It stores the episodes, all the states that come in between the initial state and the terminal state. This is later used by the agent for learning by experience. The class supports methods for storing episodes in memory, predicting the next action based on the current environment state, and returning input and targets from memory based on specified data size.
 
 I was also provided a complete implementation to build a neural network model in the TreasureHuntGame Jupyter notebook, though it is a skeleton implementation and a Q-Training Algorithm needs to be created.
 
 The Code that I created is the implementation of a Deep-Q Learning neural network to find the best possible navigation sequence that results in reaching the treasure cell while maximizing the reward. Once the code was completed, the agent was trained using this algorithm to achieve a 100% win rate, which was successfully reached at epoch 107. 

## What do computer scientists do and why does it matter?
Computer scientists do amazing complex work that impacts nearly every aspect of modern life. They design software application or develop new technologies, use their analytical and technical skills to achieve amazing goals not only in the computer science relm, but medicine and buisness as well. The knowledge gained in algorithms, data structures, and programming languages can create new developments in AI that will in result in breakthrus in medicine and science. The ability to use AI to detect cancer at such a early stage that any type can potentially treated or cured. Using AI in a buisness to discover unknown patterns and help the buisness grow, all while streamlineing the process and making the organization more efficient. Essentially, computer scientists are the architects of the modern digital world that we all benefit from.

## How do I approach a problem as a computer scientist?
First I establish the reason behind the problem and research on ways to better the situation. Once a solid plan has been found, I break the process down into smaller tasks, and make alterations as the process unfolds. For the Pirate Game project, the goal is clear, make the intellegent agent find the goal. Then I designed a Deep Q-learning network and implemented the solution. Once the test was ran successfully, I made the neccessary adjustments and came to a final product. This is similar to an Aglie approach. Plan (which was provided for me), Design (decision on using a DQN), Develop (create the nessesary code), Test (multiple tests were run to determine the final product), Deploy, and Review. Although the game was never deployed. 

## What are my ethical responsibilities to the end user and the organization?
My ethical responsibilites to the end user and the organization coincide with the General Data Protection Regulation (GDPR) law, which are as follows:

**Lawfulness, fairness and transparency** - Processing must be lawful, fair, and transparent to the data subject.

**Purpose limitation** - You must process data for the legitimate purposes specified explicitly to the data subject when you collected it.

**Data minimization** - You should collect and process only as much data as absolutely necessary for the purposes specified.

**Accuracy** - You must keep personal data accurate and up to date.

**Storage limitation** - You may only store personally identifying data for as long as necessary for the specified purpose.

**Integrity and confidentiality** - Processing must be done in such a way as to ensure appropriate security, integrity, and confidentiality (e.g. by using encryption).

**Accountability** - The data controller is responsible for being able to demonstrate GDPR compliance with all of these principles.
##
For more information about the GDPR, please check out [GDPR.EU](https://gdpr.eu/)
