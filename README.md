# Client-server hangman project in Advanced Programming course

In this group project, we were asked to implement a TCP/IP client-server program in C where the client would be playing the hangman game with the server.

Server:
1) Receives port number and reads .txt file that contains the game dictionary from command line. 
2) Chooses a random word from the dictionary and informs client about the number of letters in the word, its first and last letter, as well as the number of attempts to find it.
3) Receives letter (attempt) from client and returns position of letter in given word, if it exists. In case of a failed attempt, server updates the hangman illustration and the remaining user attempts.

Client:
1) Receives IP address and port number from command line and connects to server.
2) Displays the information given by the server to the screen and asks user to enter a letter.
3) If user finds the word or exceeds the allowed number of attempts, client displays respective message and terminates its execution.


This repository contains:
- Game dictionary (.txt file)
- Server code (.c file)
- Client header file (.c file)
