# MAPD-using-AI
Simulation of a maze solving bot that would learn the maze path during the first run and calculate the shortest path between the start and end and would follow that shortest path in all the subsequent runs

Logic:
The bot traverses the entire maze and creates a string that stores all the recorded directions.
r-Right | l-Left | f-Forward | b-Back
An example string can be rbfbrbfbl
This string is then operated upon within this algorithm so as to reduce it such that consecutive fb,bf,lr,rl are eliminated
The algorithm continues to reduce the string until the string cannot be reduced any further
Example process for - rbfbrbfbl -> rbrbl -> This string cannot be further reduced thus this is the shortest path that the bot would follow for all its subsequent runs
