# 9×9 Multiplication Battle
9×9 Multiplication Battle is a simple educational battle game created with Microsoft MakeCode Arcade. This project was made for the UTS 52685 Creative Coding Course.
The game combines multiplication practice with a chase and battle system. Helps young children strengthen the 9×9 multiplication table. The player controls a blue character while a yellow enemy follows them. When the enemy touches the player, a multiplication question appears.

Play it here: https://arcade.makecode.com/S00555-74045-05842-49322


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Features](#features)
* [Screenshots](#screenshots)
* [Setup](#setup)
* [Code files](#codefiles)
* [Usage](#usage)
* [Project Status](#project-status)
* [Room for Improvement](#room-for-improvement)
* [Acknowledgements](#acknowledgements)
* [References](#references)
* [Contact](#contact)
<!-- * [License](#license) -->


## General Information
- When I was in primary school in China, memorising the 9×9 multiplication table felt difficult and repetitive.
- My younger brother is about to start primary school, so I wanted to make this practice more fun for him.
- In this game, every attack is earned by answering a multiplication question, so playing is also practising.
- This was my first coding project. I built it to learn how code connects questions, player input, health and game results.


## Technologies Used
- Microsoft MakeCode Arcade
- MakeCode Blocks
- MakeCode Arcade simulator for testing and debugging
- Status Bars extension for the enemy health bar

## Features
- Random multiplication questions using numbers from 1 to 9
- Blue player controlled with the arrow keys
- Yellow enemy that follows the player
- Player starts with 5 lives
- Enemy starts with 10 health points
- A correct answer removes 1 enemy health point
- A wrong answer removes 1 player life
- 5 correct answers in a row trigger a Super Attack
- Super Attack removes 4 extra enemy health points
- A fire effect shows when the Super Attack is used
- When enemy health reaches 5 or lower, the enemy changes into an Angry Enemy
- Enemy speed increases from 40 to 55 when its health is low
- Win and lose screens with visual effects

  Design Choices for Younger Players
- 5 lives to make mistakes less discouraging.
- 2 digit answers because the highest answer is 81.
- A 1.5 second pause after each question gives the player time to move away.


## Screenshots
### MakeCode Blocks and Multiplication Question<img width="2816" height="1540" alt="屏幕截图 2026-10-26 011006" src="https://github.com/user-attachments/assets/bb55daa0-2c10-4523-b86f-3fe7f9dd8790" />

The game uses random multiplication questions, answer checking, health values and a streak system.

## Screenshots
<img width="696" height="958" alt="屏幕截图 2026-10-23 012349" src="https://github.com/user-attachments/assets/73082a84-27dc-4151-9d1b-0ae20882d9c2" />

The Super Attack is triggered after 5 correct answers in a row. The enemy also changes appearance when its health becomes low.


## Setup
No local installation is required.
To open the project in MakeCode Arcade:
- Go to Microsoft MakeCode Arcade.
- Click Import.
- Select Import URL.
- Paste the URL of this GitHub repository.
- Open the project and run it in the MakeCode Arcade simulator.


## Code Files

- `main.blocks` – the Blocks version of the game code, which can be opened in MakeCode.
- `main.ts` – the JavaScript version of the game code. with comments explaining each part
- `assets.json`, `images.g.jres`, `images.g.ts` – game sprites and background images.
- `pxt.json` – project settings and extensions.


## Usage
This game is designed for practising multiplication from 1×1 to 9×9.

### How to Play
1. Use the arrow keys to move the blue player.
2. When the enemy touches the player, a multiplication question appears.
3. Enter the correct answer to damage the enemy.
4. A wrong answer removes one player life.
5. Get 5 correct answers in a row to trigger a Super Attack.
6. Reduce the enemy's health to 0 to win the game.

### Code Example
    if (playerAnswer == firstNumber * secondNumber) {
        // A correct answer damages the enemy and adds 1 to the correct answer streak.
        enemyHPBar.value += -1
        streak += 1}


## Project Status
Project is: complete (submitted as my A2 prototype for 52685 Creative Coding).


## Room for Improvement
Room for improvement:
- Show a friendly "Try again!" message when the player loses. I tried this, but it did not look right, so I kept the game simple for now.
- Add a lose sound so the win and lose screens feel more consistent.

To do:
- Add a pixel pet reward after winning.
- Add more difficulty levels, such as stronger enemies or harder questions.


## Acknowledgements
- Built with Microsoft MakeCode Arcade.https://arcade.makecode.com/#
- I used the MakeCode Arcade Pizza Party tutorial while learning basic MakeCode blocks: https://arcade.makecode.com/#tutorial:/tutorials/chase-the-pizza
- The project uses the MakeCode Status Bars extension by jwunderl: https://github.com/jwunderl/pxt-status-bar


## Reference
- Microsoft. (n.d.). Microsoft MakeCode Arcade. https://arcade.makecode.com/
- Łyczywek, R. (2018, October 15). How to write a good README for your GitHub project? Bulldogjob.com; Bulldogjob. https://bulldogjob.com/readme/how-to-write-a-good-readme-for-your-github-project
- ritaly. (2018). GitHub - ritaly/README-cheatsheet: Template for a clear GitHub README (markdown). GitHub. https://canvas.uts.edu.au/courses/41840/pages/git-repository


## Contact
Tongyu Zhou
UTS 52685 Creative Coding-Tutorial 7
