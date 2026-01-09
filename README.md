This project is a Reaction testing game, where you can test your reaction time. When initially started, it displays "Click to Start" in which if the user click the button, the game begins. After the button is pressed, the next display is "Click whenGreen" which starts a randomized timer for the green LED to turn on. When the timer ends, and the green LED turns on, a stopwatch is started until the user presses the button one more time. After the time is stopped, the screen will display "elapsed time = X:XXX" and will stay on screen until user presses button 3 times. After the button is pressed 3 times, the screen will display "Click to Play Again." If the user pressees the button again, it will bring the user back to "Click when green" and repeat the cycle.
Design process:
Define a problem: People want a fun and easy way to practice, measure, and train their reaction speed. My target audience would be people of all ages, as this would be accessible to anyone. The solution is to create a game that randomly turns the green LED on, and you are supposed to click the button as soon as it turns green. And if you do it too slow, it would say too slow, try again, and if it was good, it would say perfect. This is the design process I drew on paper two days ago:
Generate concepts: I then start researching different projects made using pitop that had to do with reaction games: 
This site is about a player v player reaction time game, which I thought was very cool https://www.pi-top.com/blog/2018/05/11/how-to-create-your-own-quick-reaction-game 
I was unable to find more videos surrounding pi-top, so I then brainstormed ideas:
Idea A: 1 player waiting until it turns green (time is random)
Idea B: 1 player waits for the countdown from red -> yellow -> green (time is always the same)
Idea C: 2 players, 2 buttons, and the first to click their button when it turns green wins. 
![IMG_8169](https://github.com/user-attachments/assets/34a212b3-a0bc-4387-b13b-27990498deba)
Version A
Pros: Unpredictable, easy to play, one player requirnment
Cons: repetitive gameplay
Version B
One player requirement, easy to play
Predictable, repetitive gameplay
Version C
Multiplayer, fun, competition
Messier, more player requirements

To conclude, I chose version A as this game was made to train your reaction time, and was made to be played anywhere.
Also, the materials I plan on using are: red LED, green LED, wires, pitop, potentiometer, and button.
Develop a solution: 
Week 1: Learning how to use Pitop and simple code.
Week 2: Doing the projects from PLTW
Week 3: Starting my planning and simple coding for the reaction project (now)
Week 4: I plan on getting the reaction gameplay down by the end of this week. I also plan on adding a second mode to add a second player.
Week 5: I plan on adding a potentiometer, which would adjust the difficulty of the game.
Week 6: This week, I will finalize my project and make sure everything works as intended. Also, I would let my classmates view and critique it for any problems.
Diagram: 
1. The start shows “Press button to start” 
2. Displays “Click when green”.
3. Wait a random amount of time.
4. Turn on green light and start timer.
5. When button is pressed, stop timer.
6. Go back to start for another round.
