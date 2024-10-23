Slot Machine Game Documentation
This Python script implements a simple slot machine game. Players can deposit money, choose how many lines to bet on, and place bets on each line. The game randomly generates a slot machine spin and calculates the winnings based on the symbols that appear. The game continues until the player decides to quit.

Constants
MAX_LINES: Maximum number of lines the player can bet on (default is 3).
MAX_BET: Maximum amount that can be bet on each line (default is 100).
MIN_BET: Minimum amount that can be bet on each line (default is 1).
ROWS: Number of rows in the slot machine (default is 3).
COLS: Number of columns in the slot machine (default is 3).
Symbol Definitions
symbol_count: A dictionary that defines the number of each symbol in the slot machine.
symbol_value: A dictionary that defines the monetary value associated with each symbol.
Functions
check_winnings(columns, lines, bet, values)
Calculates the total winnings based on the symbols displayed in the columns and the player's bet.

Parameters:
columns: A list of lists representing the slot machine's columns.
lines: The number of lines the player has bet on.
bet: The amount bet on each line.
values: A dictionary containing the value of each symbol.
Returns:
winnings: Total winnings calculated.
winning_lines: A list of lines on which the player won.
get_slot_machine_spin(rows, cols, symbols)
Generates a random spin for the slot machine.

Parameters:
rows: Number of rows in the slot machine.
cols: Number of columns in the slot machine.
symbols: A dictionary containing the count of each symbol.
Returns: A list of lists representing the columns of the slot machine after the spin.
print_slot_machine(columns)
Prints the slot machine's current state in a user-friendly format.

Parameters:
columns: A list of lists representing the columns of the slot machine.
deposit()
Prompts the user to deposit an amount of money into their account.

Returns: The amount deposited as an integer.
get_number_of_lines()
Prompts the user to select the number of lines to bet on.

Returns: The number of lines selected as an integer.
get_bet()
Prompts the user to enter the amount they wish to bet on each line.

Returns: The amount bet as an integer.
game(balance)
Handles a single round of the slot machine game.

Parameters:
balance: The current balance of the player.
Returns: The net change in balance after the game round.
main()
The main function that initializes the game, manages user interactions, and maintains the player's balance.

Usage Instructions
Run the Script: Execute the script in a Python environment.
Deposit Money: Follow the prompt to deposit an amount greater than zero.
Select Lines: Choose the number of lines to bet on (1 to 3).
Place Bet: Enter the bet amount for each line (between $1 and $100).
Play the Game: Press Enter to spin the slot machine. The results will be displayed, and winnings (if any) will be calculated.
Repeat or Quit: You can continue playing or quit by pressing 'q'.
