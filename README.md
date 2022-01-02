# BashBingoCard
Play bingo on Linux.

This program takes a file as a CLA that must be of the following format:
- an integer seed line (line 1)
- a bingo card, each value being 2 digits (lines 2-6)

The bingo card must have the following format:
- column 1 contains 5 unique integers in [01-15]
- column 2 contains 5 unique integers in [16-30]
- column 3 contains 4 unique integers in [31-45] plus middle integer 00
- column 4 contains 5 unique integers in [46-60]
- column 5 contains 5 unique integers in [61-75]  

Card numbers must have exactly 2 digits, and be separated by one space,
with no extraneous whitespace, not even at the start or end of a line.  
All card number MUST be unique as well, no duplicates.

The card can have no extra lines, else it wil throw an error.

Example of a valid file contents:  
168  
01 25 40 59 75  
04 19 34 46 70  
07 17 00 52 68  
15 30 41 50 61  
09 21 45 49 67  

To run:
Take the LINUX file and make it executable.  
In the same directory, have a file that has contents that meet the reqirements above.  

On the terminal, run the program by running ./LINUX [Your file]  

If everything works, you should have a screen that looks like this (check the raw to be able to see the proper formating of the game below):  

CALL LIST:  
 L   I   N   U   X  
01  25  40  59  75  
04  19  34  46  70  
07  17  00m 52  68  
15  30  41  50  61  
09  21  45  49  67  
Enter any character to continue, or q to quit:  
