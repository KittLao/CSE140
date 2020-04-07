# CSE140

Pacman project for Introduction to Artificial Intelligence class. All my code done in student folder.

All testing command lines shows here.

# Part 1

Code written in search.py and searchAgents.py

# Depth First Search:

python3 -m pacai.bin.pacman --layout tinyMaze --pacman SearchAgent --agent-args fn=pacai.student.search.depthFirstSearch

python3 -m pacai.bin.pacman --layout mediumMaze --pacman SearchAgent --agent-args fn=pacai.student.search.depthFirstSearch

python3 -m pacai.bin.pacman --layout bigMaze --pacman SearchAgent --agent-args fn=pacai.student.search.depthFirstSearch

# Breadth First Search:

python3 -m pacai.bin.pacman --layout mediumMaze --pacman SearchAgent --agent-args fn=pacai.student.search.breadthFirstSearch
python3 -m pacai.bin.pacman --layout bigMaze --pacman SearchAgent --agent-args fn=pacai.student.search.breadthFirstSearch

# Uniform Cost Search:

python3 -m pacai.bin.pacman --layout mediumMaze --pacman SearchAgent --agent-args fn=pacai.student.search.uniformCostSearch

python3 -m pacai.bin.pacman --layout mediumDottedMaze --pacman StayEastSearchAgent

python3 -m pacai.bin.pacman --layout mediumScaryMaze --pacman StayWestSearchAgent

# A* Search:

python3 -m pacai.bin.pacman --layout bigMaze --pacman SearchAgent --agent-args fn=pacai.student.search.aStarSearch,heuristic=pacai.core.search.heuristic.manhattan

# Finding All Corners

python3 -m pacai.bin.pacman --layout tinyCorners --pacman SearchAgent --agent-args fn=pacai.student.search.breadthFirstSearch,prob=pacai.student.searchAgents.CornersProblem

python3 -m pacai.bin.pacman --layout mediumCorners --pacman SearchAgent --agent-args fn=pacai.student.search.breadthFirstSearch,prob=pacai.student.searchAgents.CornersProblem

python3 -m pacai.bin.pacman --layout mediumCorners --pacman AStarCornersAgent

--pacman SearchAgent --agent-args fn=pacai.student.search.aStarSearch,prob=pacai.student.searchAgents.CornersProblem,heuristic=pacai.student.searchAgents.cornersHeuristic

# Eating All The Dots

python3 -m pacai.bin.pacman --layout trickySearch --pacman AStarFoodSearchAgent

# Suboptimal Search

python3 -m pacai.bin.pacman --layout bigSearch --pacman ClosestDotSearchAgent

# Part 2

# Reflex Agent

python3 -m pacai.bin.pacman --pacman ReflexAgent --layout testClassic

python3 -m pacai.bin.pacman --pacman ReflexAgent --num-ghosts 1

python3 -m pacai.bin.pacman --pacman ReflexAgent --num-ghosts 2

# Minimax

python3 -m pacai.bin.pacman --pacman MinimaxAgent --layout minimaxClassic --agent-args depth=4

python3 -m pacai.bin.pacman --pacman MinimaxAgent --layout trappedClassic --agent-args depth=3

# Alpha Beta Agent

python3 -m pacai.bin.pacman --pacman AlphaBetaAgent --agent-args depth=3 --layout smallClassic

# Expectimax Agent

python3 -m pacai.bin.pacman --pacman AlphaBetaAgent --layout trappedClassic --agent-args depth=3 --null-graphics --num-games 10

python3 -m pacai.bin.pacman --pacman ExpectimaxAgent --layout trappedClassic --agent-args depth=3 --null-graphics --num-games 10

# Evaluation Function

python3 -m pacai.bin.pacman --layout smallClassic --pacman ExpectimaxAgent --agent-args evalFn=pacai.student.multiagents.betterEvaluationFunction --null-graphics --num-games 10

# Part 3

# Value Iterations

python3 -m pacai.bin.gridworld --agent value --iterations 100 --episodes 10

python3 -m pacai.bin.gridworld --agent value --iterations 5

# Bridge Grid

python3 -m pacai.bin.gridworld --agent value --iterations 100 --grid BridgeGrid --discount 0.9 --noise 0.2

# Discount Grid

python3 -m pacai.bin.gridworld --agent value --iterations 100 --grid DiscountGrid --discount 0.9 --noise 0.2 --living-reward 0.0

# Q-Learning

python3 -m pacai.bin.gridworld --agent q --episodes 5 --manual

python3 -m pacai.bin.gridworld --agent q --episodes 100

python3 -m pacai.bin.gridworld --agent q --episodes 50 --noise 0 --grid BridgeGrid --epsilon 1

python3 -m pacai.bin.crawler

# Approximate Q-Learning and State Abstraction

python3 -m pacai.bin.pacman -p PacmanQAgent --num-training 2000 --num-games 2010 --layout smallGrid

python3 -m pacai.bin.pacman -p PacmanQAgent --num-games 10 --layout smallGrid --agent-args numTraining=10

python3 -m pacai.bin.pacman -p ApproximateQAgent --num-training 2000 --num-games 2010 --layout smallGrid

python3 -m pacai.bin.pacman -p ApproximateQAgent --agent-args extractor=pacai.core.featureExtractors.SimpleExtractor --num-training 50 --num-games 60 --layout mediumGrid

python3 -m pacai.bin.pacman -p ApproximateQAgent --agent-args extractor=pacai.core.featureExtractors.SimpleExtractor --num-training 50 --num-games 60 --layout mediumClassic





