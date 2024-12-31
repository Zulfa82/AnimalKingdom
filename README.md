This project is developed as a part of the Final assessment for the Software development subject of MIT

This assignment will give you practice with defining classes. You are to write a set of classesthat define
the behavior of certain animals. You will be given a program that runs a simulation of a world with
many animals wandering around in it. Different kinds of animals will behave in different ways and you
are defining those differences.
For this assignment, you will be given a lot of supporting code that runs the simulation.
Every object in this world is a "critter", where Critter is the super class with default behavior defined.
You will be writing five classes, each representing a different type of Animal: Bear, Tiger, WhiteTiger,
Giant and NinjaCat. All of the classes you right should be sub classes of Critter. On each round of the
simulation, each critter is asked for 3 pieces of information:
1. How should it act?
2. What color is it?
3. What string represents that critter?
These 3 pieces of information are provided by 3 methods present in each Critter class. You will be
responsible for overriding these methods and programming their appropriate behavior:
THE METHODS
getColor()
As the simplest method, we suggest you start writing the getColor() method first. For getColor you
should return whatever color you want the simulator to use when drawing your critter. Colors are
represented like "Color.WHITE". For the random colors, each possible choice must be equally likely.
You may use either a Random object or the Math.random() method. If your color changes based on
moves, you will want some way to count how many moves a critter has made. This state should only
be updated in the getMove method, and simply referenced in others (like getColor or toString).
toString()
For the toString method, you should return whatever text you want the simulator to use when
displaying your critter (normally a single character). Remember, that if your String changes based on
moves you might need to keep track of the critter’s number of moves. For this assignment, do not
worry about integer overflow (we won’t run the simulation that long).
Then critters of that type will be included in the simulation.
The simulator provides great visual feedback about where critters are, so you can watch them move
around the world. But it doesn’t give great feedback about what direction critters are facing. The
simulator has a "debug" button that makes this easier to see. When you request debug mode, your
critters will be displayed as arrow characters that indicate the direction they are facing.
The simulator also indicates the "step" number as the simulation proceeds (initially displaying a 0).
