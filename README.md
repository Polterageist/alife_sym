# alife_sym
#1. ABOUT
Home project of a-life, genetic programming, neural networks and other AI-relational experiments in modeled environment. The subject of this project is modeling of some simplified "world", with its rules and living in ai creatures (so called bot's). Creatures are driven by various agent behaviour methods, like neuronal networks or simple VM. The system simulates changes in their behaviour by genetic algorithm. 

#1. THE WORLD 
The world is the grid, closed onto itself by sides (like torus surface). Each grid cell can contain one of this things:
* The wall
* The bot
* The food
* The void
Initial world state generates randomly and changes after start. Walls blocks bot's movement, so they can't step on this cell. The food increases bot's life. 
Bots itself has their life property, which is decreases by time. Their state is defined by their life, current turn (UP, LEFT, DOWN, RIGHT), perception of front cell (which object is there), and signal sensor (1 byte integer). They can turn, move, wait, percept world's state, attack, communicate or mate with each other.
