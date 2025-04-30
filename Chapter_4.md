<div style='text-align: justify;'>

# Knowledge and Reasoning
## Knowledge Based Agent
![alt text](image-5.png)

### Architecture of a KB Agent:  

1) **Knowledge Level**:
    - It is the most abstract level of agent implementation. 
    - The knowledge level describes the agent based on what it knows. This is what knowledge the agent has as the initial knowledge.
    - Basic data structures and procedures to access that knowledge are defined in this level
    - Agents at the knowledge level can be viewed as an agent for which one only need to specify what the agent knows and what its goals are in order to specify its behaviour, regardless of how it is to be implemented.  

2) #### Logical Level:
    - At the logical level, the knowledge is encoded into sentences. This level uses some formal language to represent the information it has.
    - Two types of representation techniques: Propositional Logic & First Order or Predicate Logic.

3) #### Implementation Level:
    - In implementation level, physical representation of logical level sentences is done. This level also describes data structures used in knowledge base and algorithms that are used for data manipulation.

The knowledge based agent must be able to perform following tasks:
- Represent states, actions, etc.
- Incorporate new precepts.
- Update internal representations of the world.
- Deduce hidden properties of the world.
- Deduce appropriate actions.

## The WUMPUS World Environment
#### WUMPUS is a map-based game. Let's understand the game :
- WUMPUS world is like a cave, which represents number of rooms, rooms, which are connected by passage ways. We will take a 4 X 4 grid to understand the game.
- WUMPUS is a monster who lives in one of the rooms of the cave. WUMPUS eats the player (agent) if player (agent) comes in the same room. Fig. 3.2.1 shows that room (3, 1) where WUMPUS is staying.
- Player (agent) starts from any random position in cave and has to explore the cave. We are starting from (1, 1) position.  

![alt text](image-6.png)
#### **There are various sprites in the game like pit, stench, breeze, gold, and arrow. Every sprite has some feature. Let's understand this one-by-one** :
- Few rooms have bottomless pits, which trap the player (agent) if he comes to that room. You can see in the Fig. 3.2.1 that room (1,3), (3,3) and (4,4) have bottomless pit. Note that even WUMPUS can fall into a pit.
- Stench experienced in a room, which has a WUMPUS in its neighbourhood room. See the Fig. 3.2.1, here room (2,1), (3,2) and (4,1) have stench.
- Breeze is experienced in a room, which has a pit in its neighbourhood room. Fig. 3.2.1 shows that room (1,2), (1,4), (2,3), (3,2), (3,4) and (4,3) consists of Breeze.
- Player (Agent) has arrows and he can shoot these arrows in straight line to kill WUMPUS.
- One of the rooms consists of gold, this room glitters. Fig.3.2.1 shows that room (3,2) has Gold.  

Apart from above features player (agent) can accept two types of percepts which are: Bump and scream. A bump is generated if player (agent) walks into a wall. While a sad scream created everywhere in the cave when the WUMPUS is killed.  

#### **Let's take a look at the actions which can be performed by the player(agent) in WUMPUS World :**
- Move : To move in forward direction,
- Turn : To turn right by 90 degrees or left by 90 degrees,
- Grab : To pick up gold if it is in the same room as the player(agent),
- Shoot : To Shoot an arrow in a straight line in the direction faced by the player (agent).  


</div>