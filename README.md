# obstacle-reinforcement
Designing an AI Agent to play the game of Object vs. Blocks

The steps of execution are as follows:

1. Building the objects need in the environment with pymunk and pygame
2. Designing the physics and movement of the of the objects using libraries form pymunk in python
3. Setting the rules/constraints for the game and the result of events that could happen.
4. After environment is made, start the training, we design a deep Neural network using Keras over TensorFLow.
5. Use the concept of learning, where the object learns from its surroundings one iteration at a time
6. We train the agent, in the environment for 100000 epochs, iterations with falling epsilon value, we train until we get a minimum epsilon value.
7. We divide the iteration into 4 parts, then we choose the part which contains the iteration with the maximum reward.
8. Finally, the agent starts dodging the objects


The most innovative component of the project is the implementation of the UI (User Interface) using pygame and pymunk (which are python libraries).
‘pymunk’ can basically be defined as a physics based library. So, pymunk basically allows components designed in pygame to be influenced by the concepts of physics.
For example, if we create a circle in pygame, next using pymunk we can define its working according to physics with concepts like:
1. Moment of Inertia
2. Rotation
3. Direction defined by Vec2D
4. Collisions

To run the code, you do the follows:

python3 learning.py : This will create models in saved_models folder

Then,

python playing.py : Change the model to be used in the code, based on the one that has maximum reward

Finally, 

python plotting.py 


Inspired from: https://github.com/harvitronix/rl-rc-car
