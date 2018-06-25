# Introduction-to-Artificial-Intelligence-Stanford-
UDACITY - Introduction to Artificial Intelligence - Stanford CS271
https://classroom.udacity.com/courses/cs271

## Artificial Intelligence 

 

Artificial intelligence is intelligence exhibited by machines, where a machine may learn to improve on it's task to better achieve its goal. In computer science, the field of AI research defines itself as the study of "intelligent agents": any device that perceives its environment and takes actions that maximize its chance of success at some goal.   

Colloquially, the term "artificial intelligence" is applied when a machine mimics "cognitive" functions that humans associate with other human minds, such as "learning" and "problem solving"  

The field was founded on the claim that human intelligence "can be so precisely described that a machine can be made to simulate it". This raises philosophical arguments about the nature of the mind and the ethics of creating artificial beings endowed with human-like intelligence, issues which have been explored by myth, fiction and philosophy since antiquity. 

The overall research goal of artificial intelligence is to create technology that allows computers and machines to function in an intelligent manner. The general problem of simulating (or creating) intelligence has been broken down into sub-problems. These consist of particular traits or capabilities that researchers expect an intelligent system to display.  

Machine learning, a fundamental concept of AI research since the field's inception,[61] is the study of computer algorithms that improve automatically through experience. 

Deep learning is a subset of Machine learning, using either neural networks or a cascading analysis method where the output of one analysis feeds into another.  

Many of the problems machines are expected to solve will require extensive knowledge about the world. Among the things that AI needs to represent are: objects, properties, categories and relations between objects; situations, events, states and time; causes and effects; knowledge about knowledge (what we know about what other people know); and many other, less well researched domains. A representation of "what exists" is an ontology: the set of objects, relations, concepts, and properties formally described so that software agents can interpret them 

 

The most general ontologies are called upper ontologies, which act as mediators between domain ontologies that cover specific knowledge about a particular knowledge domain (field of interest or area of concern). Such formal knowledge representations are suitable for content-based indexing and retrieval, scene interpretation, clinical decision support, knowledge discovery via automated reasoning. 

History: 

Started in the Summer of 1956 

Research kickoff at Dartmouth – Can we make computers execute reasoning tasks? 

Marvin Minsky (Foundational work in Neural Networks – Perceptrons) (MIT) 

John Mcarthy (Inventor of LISP) (MIT) 

Claude Shannon (Father of Information Theory) [self navigating mouse in maze, chess AI] 

Nathaniel Rochester 

Allen Newell (CMU),  
[Information Processing Language (1956) and two of the earliest AI programs, the Logic Theory Machine (1956) and the General Problem Solver (1957) (with Herbert A. Simon).]  

Herbert Simon (CMU), [Co-author with Allen Newell, economist, cognitive science and decision science proponent] 

Arthur Samuel (IBM) [Coined the term Machine Learning in 1959, made the first Checkers AI with IBM] 

Teach computers to represent knowledge of the real world 

What are objects? People? Language? 

How to understand language through context? 

First self driving robot invented in SRI Menlo Park in the 1960's 

First IBM mainframe at George Town University to translate Russian to English and back. 

In the late 1990s and early 21st century, AI began to be used for logistics, data mining, medical diagnosis and other areas. The success was due to increasing computational power (see Moore's law), greater emphasis on solving specific problems, new ties between AI and other fields and a commitment by researchers to mathematical methods and scientific standards. Deep Blue became the first computer chess-playing system to beat a reigning world chess champion, Garry Kasparov on 11 May 1997 

The AI Sector faced Boom/Bust cycles called AI Winters  

1966: the failure of machine translation, 

1970: the abandonment of connectionism, 

1971–75: DARPA's frustration with the Speech Understanding Research program at Carnegie Mellon University, 

1973: the large decrease in AI research in the United Kingdom in response to the Lighthill report, 

1973–74: DARPA's cutbacks to academic AI research in general, 

1987: the collapse of the Lisp machine market, with the introduction of more affordable microcomputers, running lisp programs even faster, removing the need for high profit margin systems. 

1988: the cancellation of new spending on AI by the Strategic Computing Initiative, 

1993: expert systems slowly reaching the bottom, and 

1990s: the quiet disappearance of the fifth-generation computer project's original goals. 

The quantum leap in AI needed to shift the industry out of AI Winter. Shift from hard coded instructions to machine learning.   

Deep learning feed data structures modelled after the human brain (neural network) to refine an attempt.  

Yan Lekun – Facebook neural network lab – Hand written post code extraction. 

Speech to text – Yoshua Benjio and Jeffery Hinton  

Jergen Smidenhuper – Recurrent short term memories 

Google – Fed youtube data, it was able to classify videos and data. Data-up approach was born 

Page Break
 

Intelligent Agents (link) 

 

An Intelligent agent can perceive the state of its environments through sensors and affects it states through its actuators.  

Functions that map sensors to actuators are called the control policy of an intelligent agent.  

AI is concerned with how the agent can make decisions that it can carry out with its actuators, based on its sensor data.  

This cycle is called the Perception-Action cycle. 

 

Applications for AI: 

 

 

 

 

 

Terminology: 

Fully vs Partially Observable 

Fully Observable – Agent is fully sufficient to make the optimal decision 

Partially Observable – All data isn't fully available, memorizing past moves will help make a better decision 

Perception – Action-Cycle: Iterations of the Environment, sensor and actuator loop within an intelligent agent. 

It is convenient to assume an environment has an internal state. 

An environment is fully observable If the sensors can see the entire state of the environment 

An environment is Partially observable if the sensors can see a fraction of the state but can use past observation memories to fill in what it cannot readily observe from the state.  

We use hidden markov models to structure internal memory. 

Deterministic vs stochastic 

Deterministic environments – your agents actions uniquely determine the outcome 

The effect of moving a piece is pre-determined 

Games with dice, like backgammon is random or stochastic as there is a certain amount of randomness involved 

Discrete vs Continuous 

Discrete – there are a finite amount of actions or options (Chess moves) 

Continuous – infinite amount of options (throwing darts) 

Benign vs Adversarial Environments 

Benign has no objective of its own 

Adversarial has an objective to 'win'. As there is an opponent to the Intelligent Agent, it must be aware of counters to its own moves.  

 

 

AI as an uncertainty management.  

What do you do when you don't know what to do? 

Reasons for uncertainty 

Sensor limits 

Ignorance 

Laziness 

Stochastic environments 

Adversaries (something blockin an obervation) 

Examples of AI 

Google: Machine translation systems.  

(50 languages, 2500 permutations) 

Used language translations in newspapers for the same articles 

 

Problem Solving: 

What steps follow the first one? 

What if there's partial observabilty ? 

Definition of the problem: 

What is the intial state? 

What is the function (actions) that take the state as input, performs actions to provide a desirable outcome. 

Action{s} = {a1, a2, a3, a4, etc} 

Result{s,a} = s' 

Goal Test{s} = 1,0 (have we arrived yet?) 

Path cost function -> s(a1) -> s(a2)-> n 

Step cost function(s,a,s') -> n 

 

Inserting image... 

Initial state: Arad 

Goal Test: being in Bucharest. All other states will return 0, only Bucharest will return 1 

All cities = state space. 

Furthest paths are called the frontier (cities in green) 

Inserting image... 

Purple = Explored states 

Frontier = Green{Lugoj, Pitesti, Fagaras, Oradea} 

Step cost = distance of each route 

Path Costt = Sum of Step costs to the destination 

 

Algorithms: 

Breadth First Search – Choose the shortest possible path 

Tree search: 

Function Tree.search(problem): 

Frontier = {[initial]} 

Loop:  

If frontier is empty: return FAIL 

Path = remove_choice(frontier) 

S = path.end 

If s is a goal: return path 

For a in actions: 

Add [path + a -> Result(s,a)] 

To frontier 

Tree.search (problme p) returns path 

Frontier = {path(p.intial)} 

Loop: 

If frontier is empty: return FAIL 

Path = remove_choice(frontier) 

S = path.end 

If GoalTest(s): return path 

For a in p.Actions(s): 

Add[path + a -> Result(s,a)] to frontier 

Why do we backtrack? 

Inserting image... 

Because the initial option was removed. We may even need to go backwards to pursue another route to get to the location.  

Inserting image... 

How do we avoid lengthening our process? We keep track of where we've been and where we haven't. What is the discovered and undiscovered. This is done by keep track of past states and avoiding going back to a previous state.  

Graph Search: 

Function graph.search(problem): 

Frontier = {[Intial]}; expand = {} 

Loop:  

If frontier is empty: return FAIL 

Path – remove_choice(frontier) 

S = path.end; add s to explored 

If s is a goal: return path 

For a in actions: 

Add [path + a-> result(s,a)] 

To frontier 

Unless Results(s,a) in frontier explored 

 

Graph search doesn't stop once it arrives at the Goal node. It might not be the best or shortest path. So it must check other paths to prove that It's the shortest path.  

 

General graph and tree search will only look at the minimum states rather than the shortest distance using the path cost.  

Uniform Cost search will find the path with the cheapest total cost 

This will pick the cheapest path first.  

Inserting image... 

Path 1: arad -> Zerind -> Oradea = 146 

Compares 146 to 140 and 118.  

Path 2: Chooses Arad -> Timisoara 

No compares to previous paths, 146, 140 and 229, it will revert to 140 

Path 3: Arad-> Sibiu 

 

Inserting image... 

Breadth first – least number of steps (2n storage) 

Cheapest First – Lowest total cost (2n storage) 

Depth first – Longest path first (n nodes) substantial storage savings 

 

Cheapest first isn't directed. It works like concentric circles. To find the goal faster, we need to add more knowledge, such as 

The distance towards the goal.  
Greedy best first search – we expand towards the goal first.   

 

Concentric circles, all paths explored before choosing the minimum unit cost to the goal.  

 

Instead of concentric circles, each past is made as close to the end goal as possible, starting from the first iteration.  

Inserting image... 

What if there's a barrier? The greedy-best first search will take a longer route thinking it's getting closer to the goal.  

To overcome the barrier nearest to us, we need to use an A* start algorithm that combines greed-best first search and uniform cost search.  

A* Algorithm: 

F = min(g+h) 

G(path) = path cost 

H(path) = h(s) = estimated distance to the goal 

Can be thought of as g = path cost so far and h = estimated distance to the goal.  

Min(h) = keeps us focussed in finding the goal 

Min(g) = keeps the path short 

 

How does it work?  

We measure the straight line distance to the goal from each node. We then expand each node to find numerous options then choose the least cost route, closest to our goal.  

Now does this always find the lowest cost path to the goal? 

Only if h < true cost 

H must never overestimate the goal 

H is optimisitic or admissable 

Generating a relaxed problem: 

Inserting image... 

Generating A relaxed problem: Taking a complex problem and relaxing the problem, allows us to introduce new operators to make the problem easier without overestimates.  

Problem solving works when 

The domain/ Environment is fully observable we must be able to see our start and finish 

Known: we need to know what our available actions are allowed 

Discrete – must be a finite number of actions to choose from 

Deterministic: we must know the result of an action 

Static: There must be nothing else that can change the world, except for our actions 

Implementation: 

An algorithm finds paths towards a given goal given the states of each action. 

A node is a datastructure that has 4 fields 

State: (end of the path) 

Action taken to get there 

Cost: Total Cost 

Parent: Pointer to another node 

We have a linked list of nodes.  

 

 

 

Problem set 1: 

Inserting image... 

Peg solitaire is a one player game with all holes filled except the middle. Aim is to clear the board like in checkers.  

It’s not partially observable – because we can see the full board 

It's not stochastic – we have deterministic moves, moves we make that determine our outcome 

Not continuous – we have finite and limited moves 

Not adversarial – we have one player with one goal 

Page Break
The loaded coin 

Inserting image... 

A loaded coin does not have a 50/50 probability, rather it's skewed on one end.  

If at any given point, the observable data is sufficient to make an optimal choice, the environment is fully observable; otherwise it's partially observable. 

If past data gives more information about the environment, the environment is partially observable. 

Stochastic is a random outcome as a unit of time 

Continuous is the opposite of discrete outcomes. Here we get one or the other outcome, I.e. disrete outcomes. 

No adversaries are in the system.  

Navigating a maze: 

Inserting image... 

Not partially observable: We can see the full maze.  

Not stochastic: there is no randomness 

Not continuous: there are finite moves, left or right, up or down. 

Not adversarial: no competition 

Search Tree Navigation: 

  

Left to right 

Breadth first: 6 

1 

 

 

2 

3 

4 

5 

6 

 

Depth first: 4 
 

1 

 

 

2 

 

 

3 

4 

 

 

Right to left 

Breadth first: 9 

1 

 

 

 

 

 

4 

3 

2 

 

 

 

 

9 

8 

7 

6 

5 

Depth first: 9 
 

1 

 

 

 

 

 

8 

5 

2 

 

 

 

 

9 

7 

6 

4 

3 

 

Search tree navigation 2 

 

Left – to - right 

Breadth First: 

1 

 

 

 

 

2 

3 

 

 

 

4 

5 

6 

 

 

7 

8 

9 

10 

 

 

Depth First: Note we never expand a node twice 

1 

 

 

 

2 

 

 

14 

3 

 

11 

15 

4 

8 

12 

16 

5 

9 

13 

 

6 

10 

 

 

7 

 

 

 

 

 

 

 

 

Right-to-left 

Breadth First: 

1 

 

 

 

 

3 

2 

 

 

 

6 

5 

4 

 

 

 

 

 

7 

 

 

Depth First: Note we never expand a node twice 

1 

 

 

 

 

2 

 

 

 

 

3 

 

 

 

 

4 

 

A* Search: 

In computer science, artificial intelligence, and mathematical optimization, a heuristic (from Greek εὑρίσκω "I find, discover") is a technique designed for solving a problem more quickly when classic methods are too slow, or for finding an approximate solution when classic methods fail to find any exact solution. 

The heuristic function is a way to inform the search about the direction to a goal. It provides an informed way to guess which neighbor of a node will lead to a goal. There is nothing magical about a heuristic function. It must use only information that can be readily obtained about a node. 

Specifically, A* selects the path that minimizes 

f(n)=g(n)+h(n) 

where n is the last node on the path, g(n) is the cost of the path from the start node to n, and h(n) is a heuristic that estimates the cost of the cheapest path from n to the goal. The heuristic is problem-specific. For the algorithm to find the actual shortest path, the heuristic function must be admissible, meaning that it never overestimates the actual cost to get to the nearest goal node. 

 

The distance to the goal is strictly underestimated, see the bottom and extreme right of the table.  

A* search creates a G() function, that explores the smallest distance for its next step 

h() = Heuristic function: Estimates the cheapest path from the goal 

 

1 

2 

3 

4 

5 

6 

a 

4 

4 

4 

3 

2 

1 

b 

3 

3 

3 

3 

2 

1 

c 

2 

2 

2 

2 

2 

1 

d 

1 

1 

1 

1 

1 

0 

 

G() = G Function : Cost of the path from the start node to n 

0 

1 

 

 

1 

2 

 

 

2 

3 

 

 

3 

 

 

 

 

f(n) = g(n) + h(n) 

We look for the minimum for f(n), so adding left and right we find the shortest path chosen by f(n) is down column 1.   

Page Break
 

Probability and Bayesian Networks 

 

Many causes for a problem. Looking at the influence diagram or Bayes net, can we diagnose the problem? 

Factoring in diagnostics, this is what our bayesian network looks like: 

 

A car is a complex system with variables you can't always easily measure. It has sensors and hidden problems. 

 

The Bayes network assists you in reasoning between observable variables to hidden causes.  

A bayes network is a compact representation of a distribution over a large probability distribution of all these variables. 

A Bayes network is composed of nodes, correspond to events that are random variables, linked by arcs, showing that child of an arc is influenced by its parent. Not in a deterministic way but a probablistic way. There are a total of 16 variables, the graph structure shows a huge probability distribution. If they're binary we have 2^16 possibilities of why the car is not starting.  

In this course, we will assume discrete binary options/variables 

We will learn to specify a Bayes network, observe the options, compute probabilities to determine an outcome. 

 

 

 

Probability 

Probabilities are used to express uncertainties, being a cornerstone of AI. 

Proabilities sum to 1, so all chances for all options add up to 1.  

 

 

What is the probability that we will obtain the same face each four times, either all heads or all tails 

1/16 = 4 heads 

Or 

1/16 = 4 tails 

= 1/16 + 1/16 = 2/16 = 1/8 

Remember  

Probability of x and y = * 

Probability of x or y = + 

 

What is the probability we have at least 3 heads out of 4 coin tosses?  

Map out the possibilities, we find 5 possibilites, each with 1/16 chance. We are after all the probabilities that we get >= 3 heads, so we're after an and option. 5 * (1/16) = 5/16 or 0.312 

Summary: 

 

P(X & y) = P(x)P(y) 

 

The initial coin flip has a probability of .5 --> 50% of the time you will get heads and the other 50% you get tails. Assuming you flipped the fair coin and got a H, you would move on to the H stacked coin and flip that one. The probability then is 0.90. So far, the probability that you will get a heads on the second time is 0.5*0.9 = .45. however, this isn't the only way to get second heads. Suppose you flipped the first time with the fair coin and got a T. From there you move on to the T stacked coin. Remember the coin only has 2 outcomes, so if 80% of the time it will be tails, then 20% of the time it will be heads. Probabilities always have to add up to 1. This is where the 1-0.8 comes from. The probability of a heads now is .5 *.2 = .1. Total probability is now .45+.1= .55 which is the answer. 

 

 

 

 

 

 
