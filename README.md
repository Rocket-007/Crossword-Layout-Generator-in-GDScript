
# Crossword-Layout-Generator-in-GDScript
Given a list of words, how would you go about arranging them into a cross word grid?


## DISCLAIMER
This port is not 100% perfect, here"s what i mean:

Given an input like this:  
![Example Output](https://github.com/Rocket-007/Crossword-Layout-Generator-in-GDScript/blob/main/screenshots/generator%20first%20exp%20input.png)

you will get this in the layout.table  
![Example Output](https://github.com/Rocket-007/Crossword-Layout-Generator-in-GDScript/blob/main/screenshots/generator%20first%20exp%20output.png)


Not much of a problem right?, but when given an input  
![Example Output](https://github.com/Rocket-007/Crossword-Layout-Generator-in-GDScript/blob/main/screenshots/generator%20first%20exp2%20input.png)

bruhh, you get this shhii...   
![Example Output](https://github.com/Rocket-007/Crossword-Layout-Generator-in-GDScript/blob/main/screenshots/generator%20first%20exp2%20output.png)


  
If you think this is what you can work with then be my guest  
otherwise head over to this [repository](https://github.com/Rocket-007/Crossword-Layout-Generator-in-GDScript-better-verson-) where i made a better one :3 

ok continue reading






## this is port on [Michael Wehar's](https://github.com/MichaelWehar/Crossword-Layout-Generator) JavaScript crossword generator



# Crossword Layout Generator - Open Source
## Introduction
A crossword consists of clues, answers, and a layout:
- The answers are the hidden words that the player is trying to guess.
- Each answer has a clue which is a sentence or phrase that helps the player to guess the associated answer.
- The **crossword layout** describes where the answers are located in a two-dimensional grid.

This crossword layout generator takes in a list of answers and outputs a crossword layout.  Our program **does not** generate the answers or the clues.

## Input and Output Format

An input is a list of answers in a JSON format.  The clues can optionally be included with the input.

Here is an example input:

`[{"clue":"that which is established as a rule or model by authority, custom, or general consent","answer":"standard"},{"clue":"a machine that computes","answer":"computer"},{"clue":"the collective designation of items for a particular purpose","answer":"equipment"},{"clue":"an opening or entrance to an inclosed place","answer":"port"},{"clue":"a point where two things can connect and interact","answer":"interface"}]`

The output is a crossword layout.  That is, we associate a position, startx, starty, and orientation with each answer.

Here is an example output:

`[{"clue":"the collective designation of items for a particular purpose","answer":"equipment","startx":1,"starty":4,"position":1,"orientation":"across"},{"clue":"an opening or entrance to an inclosed place","answer":"port","startx":5,"starty":4,"position":2,"orientation":"down"},{"clue":"that which is established as a rule or model by authority, custom, or general consent","answer":"standard","startx":8,"starty":1,"position":3,"orientation":"down"},{"clue":"a machine that computes","answer":"computer","startx":3,"starty":2,"position":4,"orientation":"across"},{"clue":"a point where two things can connect and interact","answer":"interface","startx":1,"starty":1,"position":5,"orientation":"down"}]`

One can visualize the output as follows:

![Example Output](https://github.com/MichaelWehar/Crossword-Layout-Generator/blob/master/example_images/crossword1_filled.png)

## Getting Started

**Step 1:** 
**Step 2:** 
```
........
...
var layout = generateLayout(input_json);
var rows = layout.rows;
var cols = layout.cols;
var table = layout.table; # table as two-dimensional array

var output_json = layout.result; # words along with orientation, position, startx, and starty
...
```

**Update:** 
## License
- MIT

## Credits

- [My channels video](https://m.youtube.com/watch?v=qC9rFCyMcl0)
