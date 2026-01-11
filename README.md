## Design Process
### Define the Problem
People with slower reaction times want a fun and easy way to practice, measure, and improve their reaction speed. Many reaction tests are either predictable or allow users to click early, which makes them less effective for training.
### Design Goal:
Create a reaction training game that:
1. Uses random timing
2. Prevents early clicking
### Generate Concepts
I started by researching different reaction-time projects made using pi-top. One project I found was a player-vs-player reaction time game, which helped me understand how timing and button inputs could be used in a reaction-based system.

After researching, I brainstormed the following ideas:

#### Idea A:

- One player waits for a green LED to turn on after a random delay

- Pros: Unpredictable, easy to play, good for reaction training

Cons: Can become repetitive

#### Idea B:

- One player waits for a countdown from red → yellow → green

- Pros: Easy to understand

- Cons: Predictable timing, less effective for training

#### Idea C:

- Two players with two buttons; first to click when green wins

- Pros: Competitive and fun

- Cons: More components and complexity

After comparing the options, I chose Idea A because it focuses on improving reaction time and can be played anywhere with minimal hardware. 
#### State Machine:
![IMG_8169](https://github.com/user-attachments/assets/34a212b3-a0bc-4387-b13b-27990498deba)
#### Block Diagram:


### Develop a Solution
#### Materials Planned:
1. Pitop
2. Button
3. Green LED
4. Red LED
5. Wires
6. Potentiometer
#### Development Plan:

Week 1: Learn how to use pi-top and write simple code

Week 2: Complete PLTW practice projects

Week 3: Plan game logic and begin coding

Week 4: Implement reaction gameplay and timing

Week 5: Add a second mode and potentiometer difficulty

Week 6: Final testing, peer feedback, and GitHub

### Final Desgin (Updated)
1. Game starts with "Click to Begin"
2. Screen displays "Click when Green"
3. If the button is pressed before green: "Too Fast"
4. If pressed after green: reaction time is displayed
5. Three button presses: return to the start up screen, displaying "Click to Play Again"
This design allows for repeated practice and prevents early-click cheating, making it effective for training.

