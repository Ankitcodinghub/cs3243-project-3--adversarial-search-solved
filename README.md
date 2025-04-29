# cs3243-project-3--adversarial-search-solved
**TO GET THIS SOLUTION VISIT:** [CS3243 Project 3- Adversarial Search Solved](https://www.ankitcodinghub.com/product/cs3243-introduction-to-artificial-intelligence-solved-3/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;114613&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS3243 Project 3- Adversarial Search Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
Overview

In this project, you will implement an adversarial search algorithm to find valid and good moves for a minichess game. Specifically, you are tasked to:

1. Implement the Alpha-Beta Pruning algorithm to play a game of minichess.

This project is worth 10% of your module grade.

General Project Requirements

The general project requirements are as follows:

• Individual project

• Python Version: 3.7

• Submission folder: LumiNUS &gt; CS3243 &gt; Projects &gt; Project 3 Submission folder

• Submission format: One standard (non-encrypted) zip file containing only the necessary project files. In particular, it should unzip to give one folder with one .py file: AB.py. More information is given in the Submission Details section below.

As to the specific project requirements, you must complete and submit the following:

• Task 1 (Alpha-Beta): Implement your Alpha-Beta Pruning algorithm in AB.py.

Note that you are tasked to implement your own board, chess pieces and states for the game. You are strongly encouraged to reuse your implementation from Project 1/2.

Background: Gardner’s Minichess

A board needs to be five squares wide to contain all kinds of chess pieces (except the pawn) on the first row. In 1969, Martin Gardner suggested a chess variant on a 5×5 board . The starting configuration of the chess board can be seen below.

Figure 1: Gardner’s 5×5 minichess

In this project, you will implement the Alpha-Beta Pruning algorithm to beat various AI agents at the game of minichess. That is, to perform a checkmate on the opposing player’s King. The rules of the game are defined in the next section.

Rules of the Minichess Game

Board Set-up

In this game, the chess pieces are divided into two different colored sets, namely White and Black. Each set consists of 10 pieces: one King, one Queen, one Rook, one Bishop, one Knight, and five Pawns.

The game is played on a square board of 5 rows and 5 columns. The rows start from row 0 at the top to row 4 at the bottom and the columns start from column ’a’ as the leftmost column to column ’e’ as the rightmost column. The White pieces are placed at rows 0 and 1 while the Black pieces are placed at rows 3 and 4. The initial configuration and position of the pieces on the board can be seen below:

Figure 2: The starting configuration of a 5×5 minichess board with rows and columns labelled.

Figure 3: The starting positions of the pieces in the 5×5 minichess.

Movement of Chess Pieces

New piece in Project 3: Pawn

• A Pawn can move forward to the unoccupied square immediately in front of it on the same column (black circle in the picture). Additionally, a Pawn can capture an opponent’s piece on a square diagonally in front of it by moving to that square (X crosses in the picture below).

• Note that we do not consider special moves for Pawns in this game (i.e., no en passant capture, no promotion, and no advancing of two squares along the same column on its first move).

Figure 4: Movement of Pawn.

• In the game in Project 3, the White Pawn can only move in the downwards direction (from row 0 to row 4) while the black pawn can only move in the upwards direction (from row 4 to row 0).

Additionally, in Project 3, we only consider the basic movements for each piece and we do not consider any special moves for any of the pieces. For example, there is no castling for Rook and no special moves for Pawns as mentioned above.

Check

When a King is under immediate attack (threatened by an opponent piece), it is said to be in check. In the standard game of chess, a move in response to a check is legal only if it results in a position where the King is no longer in check (i.e., the player cannot make any other move unless its King is taken out of the check). This can involve capturing the checking piece; interposing a piece between the checking piece and the King (which is possible only if the checking piece is a Queen, Rook, or Bishop and there is a square between it and the King); or moving the King to a square where it is not under attack.

Figure 5: Black King at e3 is checked by White Queen at b3.

Checkmate (Winning Conditions)

The objective of the game is to checkmate the opponent; in this variant, there are multiple ways to checkmate an opponent.

1. Standard Checkmate: This occurs when the opponent’s King is in check, and there is no legal way to get it out of check. Since it is illegal for a player to make a move that puts or leaves its own King in check, if it is not possible to get its King out of check, then the player cannot make any other moves and the King is considered checkmated (and the game is over).

Figure 6: White King at d0 checkmated by Black Rook at b0. Moving to d1 will cause it to be threatened by Black King at e2, so the White King cannot escape check.

2. Out of Valid Moves: This occurs when the opponent cannot make any valid moves during his turn, as any move made by the opponent will cause its King to be placed in check, resulting in a self-checkmate in the next turn as we can capture his King piece.

Figure 7: While White King at d0 is not checked now, White cannot make any more valid moves as moving his King at d0 (the only White piece left) will cause his King to be checked by the Black pieces (c0 threatened by Black Pawn at b1; c1, d1 and e1 threatened by Black King at d2; e0 threatened by Black Bishop at b3).

3. King Capture: This occurs when the opponent makes a move that will cause his King to be in check, or when his King is in check but he ignores it and makes a move that will cause his King to remain in check.

Figure 8: Black King at e4 is checked by White Queen at d3. It is now Black’s turn to move. (1/3)

Figure 9: However, Black ignores the checking White Queen and moves its King from e4 to d4, causing his King to remain in check by White Queen at d3. (2/3)

Figure 10: White Queen at d3 proceeds to capture Black King at d4, leading to White winning the game. (3/3)

Draw

In this game, we only consider the game to be a draw if White and Black have the same number of pieces left after 50 consecutive moves. This means that there is no change in the number of pieces in the board for 50 moves in a row, implying a Draw. Furthermore, this can only occur if both Kings are s till left on the board.

Additionally, we consider a game a draw if there are no more available moves for a player. For this scenario to happen, the player’s pieces must not have any free moves it can make, regardless of whether a move will place its King in check.

Figure 11: White cannot make any more moves as the King is trapped by 3 of its pawn and all of the pawns are not able to move as well. This results in a draw.)

Getting Started

You are given one python file (AB.py) with the recommended empty functions/classes to be implemented. Specifically, the following are given to you:

1. studentAgent(gameboard): DO NOT REMOVE THIS FUNCTION. This function takes in a parameter gameboard. When called, this function must return a valid Move. The output will be used to make a move on the game. More details on the output will be given in the later sections.

You are encouraged to write other helper functions to aid you in implementing the algorithms. During testing, studentAgent(gameboard) from AB.py will be called by the autograder.

Winning a minichess game using Alpha-Beta Pruning

The objectives of this part of the project are:

1. To gain exposure in the implementation of algorithms taught in class.

2. To learn to apply Minimax in games.

3. To learn the efficiency and importance of using Alpha-Beta Pruning.

Project 3 Task 1

Background:

• Dummy Agent (Testcase 1): This agent chooses the first available move that it sees and performs the action. It does not care if the move will cause its King to be checked.

• Random Agent (Testcase 2): This agent chooses a random move out of all the available moves that it sees and performs the action. It does not care if the move will cause its King to be checked.

• Greedy Agent (Testcase 3): This agent will choose a move based on a priority. Firstly, it will choose a move that will checkmate your King if there exists such a move. If there is no such move, it will then find and choose a move that will check your King. If there is no such move, it will choose any available move at random that does not cause its own King to be checked. If no such move exist, the Greedy Agent have lost by the condition of Out of Valid Moves.

• Smart Agent (Testcase 4): This agent will choose a move based on a utility value. It will pick the move that gives the highest utility. In general, a move that checkmates its opponent yields the highest utililty, followed by moves that checks its opponent’s King AND capture another piece simultaneously, followed by moves that capture another piece ONLY and lastly, moves that checks its opponent’s King ONLY. Capturing different types of piece gives different utility value as well. Additionally, If there are no valid moves that will not cause the Agent’s King to be checked, the Smart Agent have lost by the condition of Out of Valid Moves.

• Minimax Agent (Testcase 5): This agent will choose a move based on the Minimax algorithm with alpha beta pruning with a depth of 4. Its evaluation function is similar to the utility of the Smart Agent (Limited depth to improve runtime).

Task 1: Alpha-Beta Pruning Algorithm

Implement the Alpha-Beta pruning algorithm in AB.py to solve the problem stated above.

Configuration file input: Use sys.argv[1] to obtain the name of the configuration file within the studentAgent() function. This has already been added for you in the template code. (Note that it is optional to read this config file as it is fixed at all times. This means that you can hardcode the initial starting positions and the board size of the game.)

The function studentAgent() takes in a parameter gameboard that is a dictionary of positions (Key) to the tuple of piece type and its colour (Value). It represents the current pieces left on the board. Example gameboard:

When the studentAgent() function is executed, your code should return a valid move in the following format:

(pos1, pos2)

The values pos1 and pos2 represent a grid index tuple, (x,y), where x is the column index (i.e., a string), and y is the row index (i.e., an integer), such that (x,y) corresponds to a specific grid cell on the board that we wish to reference. The move specifies that you wish to move the piece at pos1 to pos2.

An example of the function output is shown below:

print(studentAgent(gameboard))

Sample output (that represents moving your White Queen at a0 to b1):

• Correct implementation of Minimax algorithm and Alpha-Beta pruning evaluated by winning or drawing against Dummy Agent consistently (100% of the time) for full credit (1m).

• Correct implementation of Minimax algorithm and Alpha-Beta pruning evaluated by winning or drawing against Random Agent consistently (100% of the time) for full credit (1m).

• Correct implementation of Minimax algorithm and Alpha-Beta pruning evaluated by winning or drawing against Greedy Agent (90% of the time) for full credit (2m).

• Correct implementation of Minimax algorithm and Alpha-Beta pruning evaluated by winning or drawing against Smart Agent (90% of the time) for full credit (2m).

• Correct implementation of Minimax algorithm and Alpha-Beta pruning evaluated by winning or drawing against Minimax Agent (80% of the time) for full credit (4m).

• Partial credits will be given and scaled proportionally based on your Agent’s performance. 10

CodePost (Platform for Running Autograder)

We will be using CodePost as our platform to run the autograder and test your code. You should have already joined the Course’s group on CodePost from Project 1. If you need any assistance for CodePost signups, please feel free to reach out and email any of the TAs.

Subsequent access: https://codepost.io/student/CS3243%20AY2122%20Semester%

202/Spring%202022/

1. Click on “Upload assignment”, and upload your python file AB.py (do NOT rename the file).

3. After the submission has been processed, refresh the page and select “View feedback”.

4. If your implementation is within CodePost’s time limit of 30s, you will see this:

Figure 12: CodePost output for Testcase 1 – 5 in a sequential order. The score shown on the left of the picture (5/5) can be disregarded.

IMPORTANT: Grading

Your code will be graded for technical correctness. Please do not change the name of the function studentAgent.

Testing of your code will be done locally. For each test case, the result of your agent will be recorded and the time taken for the execution of your code will be measured as well. To ensure that we can measure your agent’s performance fairly, your agent will play against each different agent for 10 iterations. Your agent should fulfil the winning conditions against the different agents to receive full credit. Additionally, the time taken for your Alpha-Beta Pruning algorithm will be compared to our solution’s benchmark. If the time taken for your code is above the time limit, it will be considered a failure of the test case. As such, you are encouraged to use efficient data structures when implementing your code (e.g., using a set/dictionary instead of a list). To account for the execution of code on different systems, we have provided additional buffers for the time limit.

In summary, to pass a test case, two conditions have to be fulfilled for your Alpha-Beta Pruning algorithm implementation. They are:

1. Fulfilling the winning conditions for the different AI agents as shown above.

2. Time taken to run your algorithm is within the time limit.

Other details

Allowed Libraries:

To aid in your implementation, you are allowed to use these Python libraries:

• CLI arguments: sys

• Data structures: queue, collections, heapq, array, copy, enum, string

• Math: numbers, math, decimal, fractions, random

• Functional: itertools, functools, operators

• Types: types, typing

Test Cases Debugging:

Based on Project 1 feedback, we have updated the Autograder and now it provides stacktrace and debug info in the tests.txt file as shown in the image below. However, in providing the stack trace and error information, we have disabled any printing, raising of exception and std.out methods in your AB.py file. This is to prevent any malicious students from printing the hidden test cases information.

Figure 13: CodePost Debug Output

Submission Details via LumiNUS

• For this project, you will need to submit 1 zip file containing 1 python file: AB.py

• Place the file in a folder, name the folder as studentNo and zip it as studentNo.zip. An example will be: A0123456X.zip.

• The format of submission is the same as Project 1 and Project 2.

• In summary, your submission file should be a zip file and when unzipped, it will contain the 1 file in a folder: A0123456Z.zip → unzip → A0123456Z folder → AB.py file. There should not be any subfolders.

• Do not modify the file names.

• Make only one submission on LumiNUS.

• Please follow the instructions closely. If your files cannot be opened or if the autograder cannot execute your code, it will be considered failing the test cases as your code cannot be tested.

• Submission folder: LumiNUS &gt; CS3243 &gt; Projects &gt; Project 3 Submission Folder
