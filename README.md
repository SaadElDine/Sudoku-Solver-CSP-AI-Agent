# Sudoku-Solver-CSP-AI-Agent
Sudoku Solver AI Agent using CSP: MRV, LCV, Forward Checking and Arc Consistency.

![image](https://github.com/SaadElDine/Sudoku-Solver-CSP-AI-Agent/assets/113860522/11fe420f-4a7c-4beb-922b-65bbdec6fa32)

# Problem Statement:
Sudoku is a popular puzzle game that has captured the hearts and 
minds of puzzle enthusiasts around the globe. Its simple rules and 
challenging gameplay make it a favorite pastime for people of all ages. 
In this project, we delve into the world of Sudoku, exploring its 
history, rules, and strategies for solving. 
Our goal is to not only understand the game at a deeper level but 
also to develop an AI-powered solver that can tackle Sudoku puzzles of 
varying difficulty levels. Through this project, we aim to showcase the 
power of artificial intelligence in solving complex logical puzzles, 
paving the way for future advancements in AI and its applications in 
gaming and problem-solving domains. 

# Algorithm CSP:
- The solver provides early detection for invalid game boards by 
checking for inconsistent domains before the solving process.
- The GUI updates in real-time to show the progress of the solver 
and highlight any incorrect user inputs in Mode 3.
- MRV is used to prioritize the selection of the next variable 
(cell) to assign a value.
- You maintain a list of unassigned variables and select the one 
with the fewest remaining legal values in its domain.
- When choosing the next variable to assign a value during 
backtracking, you prioritize the variable with the minimum 
remaining values.
- MRV helps the solver explore the search space more 
efficiently by selecting variables with fewer options first, 
potentially leading to faster solutions.
- LCV is used to prioritize the order in which values are 
assigned to a variable.
- For each value in the domain of a variable, you count how 
many values in neighboring variables' domains would 
become invalid if that value was chosen.
- The value with the least impact on neighboring variables is 
chosen first.
- When selecting a value to assign to a variable, you prioritize 
the values based on their impact on neighboring variables' 
domains.
- LCV helps the solver make more informed decisions about 
which values to assign, potentially reducing the likelihood of 
reaching dead-end branches in the search tree.
- Forward Checking is used to prune the domains of 
neighboring variables after a variable is assigned a value.
- When a variable is assigned a value, you check its constraints 
with neighboring variables and remove any conflicting values 
from their domains.
- After assigning a value to a variable, you update the domains 
of neighboring variables using forward checking.
- Forward Checking helps the solver reduce the search space 
by eliminating values that are no longer viable after a 
variable is assigned, potentially speeding up the solving 
process.


![image](https://github.com/SaadElDine/Sudoku-Solver-CSP-AI-Agent/assets/113860522/27a73fe3-99ab-4c66-add1-72ebbd14f88d)

![image](https://github.com/SaadElDine/Sudoku-Solver-CSP-AI-Agent/assets/113860522/2b83078a-ff49-46f8-a7e2-68f9c1c0e11f)

![image](https://github.com/SaadElDine/Sudoku-Solver-CSP-AI-Agent/assets/113860522/0fdd9fcd-eac0-4756-ae24-f9eb4e2d8520)

![image](https://github.com/SaadElDine/Sudoku-Solver-CSP-AI-Agent/assets/113860522/47a837ba-c4a3-4c7f-bca2-6291c8aec0ad)

![image](https://github.com/SaadElDine/Sudoku-Solver-CSP-AI-Agent/assets/113860522/0648eb8d-8304-49e8-94a3-e99e548b655a)

![image](https://github.com/SaadElDine/Sudoku-Solver-CSP-AI-Agent/assets/113860522/6a7e1b08-8244-4087-92ec-cdb5b7352228)

![image](https://github.com/SaadElDine/Sudoku-Solver-CSP-AI-Agent/assets/113860522/96475797-a360-4e21-b681-ce837ec85e2c)

![image](https://github.com/SaadElDine/Sudoku-Solver-CSP-AI-Agent/assets/113860522/e3f2abd4-4904-4b7c-bbed-b62917a75840)

# Conclusion:
In conclusion, the Sudoku game with CSP implementation 
successfully meets the requirements outlined for the project. The game 
features a user-friendly GUI that allows for interaction and showcases 
the AI agent's solving capabilities in Three modes: one where the AI 
agent demonstrates its solving process, another where users can input 
their own puzzles for the AI agent to solve and the interactive mode.
The CSP Sudoku solver effectively models the puzzle as a 
constraint satisfaction problem, using backtracking to validate and 
generate puzzles and arc consistency to ensure a valid solution. The 
implementation demonstrates a solid understanding of constraint 
satisfaction problems and their application to Sudoku puzzles.
The documentation and reporting requirements have been met with 
well-commented code and a report detailing the implementation, sample 
runs, and performance metrics. The addition of the bonus feature for 
early detection of invalid game boards adds extra functionality to the 
game.
In addition to the integration of Minimum Remaining Values
(MRV), Least Constraining Value (LCV), and Forward Checking 
algorithms into the Sudoku solver has significantly improved its 
efficiency and effectiveness. These techniques prioritize variable 
selection based on the fewest remaining legal values, optimize the order 
of value assignment to minimize impact on neighboring variables, and 
prune domains to reduce the search space. 
As a result, the solver is now more robust, efficient, and capable of 
solving a wide range of Sudoku puzzles
Overall, the implementation shows a strong grasp of the concepts 
involved in solving Sudoku puzzles











