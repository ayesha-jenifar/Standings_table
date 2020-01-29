# Standings_Table
This program takes inputs such as Team name, goal and updates the print table depending on the win-ner of the match. My goal was to develop the easy solution to update the team information and sort them in the point table accordingly. I tried to do some experiments with this assignment such as to implement header function of my own.
Design: The program provides four Menu driven options
1. Add Scores
2. Print Standing Table
3. Clear Screen
4. Exit
User can choose only these three options otherwise program will give print warning message. The input from the user is taken as string input and if user provides lower character alphabet then it is converted into upper character thus the input can be easily compared with the predefined menu.
1, ADD Score: The string input from the user is compared with the four-menu option. If the us-er’s input become equal to “ADD" then welcome message is printed by calling the print_add_banner function. After that, the program asks to provide the match information such as team name, goal numbers. Then the user input is checked and if wrong input is provided other than char string then it will give error message to give right input. The team name is also con-verted into upper character.
During the first entry of the team it will add directly to the table with add_team_in_table other-wise it checks whether the team is already existed in the table or not with check_team_in_table. This function returns the matched team’s index which is used to record the goals, match winner, point table. The winner of the match is determined by the goal given by the home team and visit-ing team.
Depending on the winner three different functions is called such as set_for_win, set_for_lost and set_for_draw. These functions set the goal records, winning and point records to the index that was found by the check_team_in_table or add_team_in_table.
3
2: Print Standing Table: The Team Standing is printed in this block. The team that has highest point will situate on the top of the table. The table also presents how many matches have been played, for and against goals numbers and also how many winning, loss and draw. The sorting is done by calling the find_maxvalue() where it returns the maximum number of the array. This function was called in a loop with point table array. After each call the maximum number was turned into 0 so that the next highest value scans be sorted.
3. Clear Screen: This block clears the screen by system (“CLS”) function. After clearing the screen, the option printed again.
4. Exit: While user writes Exit then it exits from the program.
