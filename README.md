# CSE140

Pacman project for Introduction to Artificial Intelligence class. All my code done in student folder.

# Part 1

Code written in search.py and searchAgents.py

Depth First Search:

python3 -m pacai.bin.pacman --layout tinyMaze --pacman SearchAgent --agent-args fn=pacai.student.search.depthFirstSearch

python3 -m pacai.bin.pacman --layout mediumMaze --pacman SearchAgent --agent-args fn=pacai.student.search.depthFirstSearch

python3 -m pacai.bin.pacman --layout bigMaze --pacman SearchAgent --agent-args fn=pacai.student.search.depthFirstSearch

Breadth First Search:

python3 -m pacai.bin.pacman --layout mediumMaze --pacman SearchAgent --agent-args fn=pacai.student.search.breadthFirstSearch
python3 -m pacai.bin.pacman --layout bigMaze --pacman SearchAgent --agent-args fn=pacai.student.search.breadthFirstSearch

Uniform Cost Search:

python3 -m pacai.bin.pacman --layout mediumMaze --pacman SearchAgent --agent-args fn=pacai.student.search.uniformCostSearch

python3 -m pacai.bin.pacman --layout mediumDottedMaze --pacman StayEastSearchAgent

python3 -m pacai.bin.pacman --layout mediumScaryMaze --pacman StayWestSearchAgent

A* Search:

python3 -m pacai.bin.pacman --layout bigMaze --pacman SearchAgent --agent-args fn=pacai.student.search.aStarSearch,heuristic=pacai.core.search.heuristic.manhattan

