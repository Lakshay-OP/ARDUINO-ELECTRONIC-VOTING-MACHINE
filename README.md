# ARDUINO-ELECTRONIC-VOTING-MACHINE
It's a Arduino based electronic voting machine project which i did in my third year of Btech. 


This project is an enhanced version of an Arduino-based voting machine, which introduces a system that not only counts votes but also gives visual feedback through an LED. The machine allows users to vote for one of three candidates or choose the NOTA (None of the Above) option. The system provides feedback by blinking an LED for 10 seconds after a vote is cast. The results of the voting process are displayed on a 16x2 Liquid Crystal Display (LCD).

Components Used
Arduino Uno: The primary microcontroller responsible for managing inputs, controlling the LCD and LEDs, and counting votes.
16x2 LCD Display: Displays voting options, thank-you messages, and the voting results.
Push Buttons: Six buttons are used:
Four for voting for candidates (P1, P2, P3) and NOTA.
One button to show results.
One button used to reset or trigger specific functionality.
LED: Used to provide visual feedback, blinking for 10 seconds after each vote is cast to simulate acknowledgment of the vote.
Resistors and Jumper Wires: Basic electronic components required for connecting the buttons, LEDs, and LCD to the Arduino.

Working Process

Voting Process:
Users can cast a vote by pressing one of the four designated buttons. A separate button is provided for each option (P1, P2, P3, and NOTA).
Upon pressing any of the voting buttons, the system displays a “Thank You” message on the LCD.
A green LED blinks for 10 seconds to acknowledge the vote, enhancing the user experience by providing a visual indicator that the vote has been registered.
After 10 seconds, the system returns to displaying the voting options, allowing for further votes to be cast.
Each vote is recorded and stored in corresponding vote counters for the options (P1, P2, P3, NOTA).

Result Display:
At any point during the voting process, pressing the results button shows the total votes for each candidate and the NOTA option.
The system evaluates which candidate received the most votes and declares the winner. If NOTA receives the highest number of votes, the LCD displays a "No One Won!" message, symbolizing dissatisfaction.
If the vote count results in a tie, the system displays a "Tie or No Result" message.
Once the results are shown, the vote counts are reset, and the machine is ready for a new voting session.

Additional Button for Special Functions:
This version of the voting machine includes a new input (sw6) for potential future expansions. Although it’s not implemented in this current iteration, it can be utilized for various purposes, such as special voting modes or administrative features.

Functionality Breakdown
Initial Setup:

Upon startup, the system displays introductory messages on the LCD encouraging users to cast their votes.
The voting options (P1, P2, P3, and NOTA) are presented on the LCD.
Voting Mechanism:

The user casts a vote by pressing a button corresponding to their chosen candidate or NOTA.
A confirmation message is displayed on the LCD, and the green LED blinks for 10 seconds as visual feedback.
Each vote is added to the total count for the corresponding candidate or NOTA.
Result Evaluation:

When the results button is pressed, the system calculates the total votes and determines the winning option.
The vote counts for P1, P2, P3, and NOTA are displayed on the LCD, and the winning candidate is announced.
If NOTA receives the highest number of votes, the system displays a message indicating no one won.
In case of a tie, a message indicating a tie or no result is shown.
Reset Function:

After displaying the results, the system resets the vote counts, readying itself for the next voting session.

Conclusion
This version of the Arduino-based voting machine enhances the voting experience by adding a 10-second LED blinking feature after each vote. The machine offers a practical way to demonstrate how votes are counted and results are evaluated, all while providing immediate visual feedback to the voter. The system is simple but versatile, with potential for expansion, such as additional voting rounds, secure voting procedures, or future functionalities through the extra button input. This project serves as an excellent foundation for understanding electronic voting systems and how they can be implemented using Arduino technology.
