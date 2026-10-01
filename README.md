🚀 Rocket vs UFO 👽

A simple browser-based shooting game developed using HTML, CSS, and JavaScript. In this game, the player controls a rocket at the bottom of the screen and shoots bullets toward a UFO. Each successful hit increases the score by one.

🎮 How the Game Works

1. The rocket starts at the bottom of the game screen.
2. Move your finger or mouse across the canvas to move the rocket left or right.
3. Tap or click on the canvas to fire a bullet.
4. The bullet travels upward toward the UFO.
5. If the bullet hits the UFO:
   - An explosion appears.
   - The score increases by 1.
   - The UFO moves to a new random position.
6. If the bullet reaches the top without hitting the UFO, it disappears.
7. The Reset button sets the score back to 0.

✨ Features

- 🚀 Touch and mouse-controlled rocket
- 🔫 Bullet shooting system
- 👽 UFO target
- 💥 Collision detection and explosion effect
- 🏆 Real-time score counter
- 🔄 Reset button
- 📱 Touch-friendly controls
- 💻 Works directly in a web browser
- 🔊 Shooting sound effect
- 🎯 Random UFO position after a successful hit

🛠️ Tech Stack

Frontend

- HTML5 – Creates the game structure and canvas.
- CSS3 – Provides the game layout and styling.
- JavaScript – Controls movement, shooting, collision detection, scoring, and game logic.

Main Components

Component| Purpose
Canvas| Game area
Rocket| Player-controlled object
UFO| Target object
Bullet| Projectile fired by the rocket
Explosion| Hit effect
Score| Displays the player's score
Reset Button| Resets the score
JavaScript| Controls game functionality

⚙️ How the Code Works

1. Game Initialization

The JavaScript creates the rocket, UFO, bullet, score, and explosion objects.

The rocket is positioned near the bottom of the canvas, while the UFO is placed near the top.

2. Rocket Movement

The player can move the rocket by moving the mouse or finger across the canvas.

The rocket's X-position is updated according to the pointer position.

The rocket is restricted so that it cannot move outside the canvas.

3. Shooting

When the player taps or clicks the canvas:

- The bullet is positioned above the rocket.
- The bullet becomes active.
- The bullet moves upward.
- A shooting sound is played.

Only one bullet is active at a time.

4. Bullet Movement

The bullet continuously moves upward during the game.

When the bullet reaches the top of the canvas, it becomes inactive and disappears.

5. Collision Detection

The program checks whether the bullet touches the UFO.

If a collision occurs:

- The bullet disappears.
- The score increases by 1.
- An explosion effect appears.
- The UFO moves to a random position.

6. Score System

The score starts at:

Score: 0

Every successful hit increases the score:

Score: 1
Score: 2
Score: 3
...

7. Reset Function

When the Reset button is clicked:

- Score becomes 0.
- The bullet is removed.
- The explosion is hidden.
- The UFO gets a new random position.

🎯 Example Actions

Player Action| Result
Move finger left| Rocket moves left
Move finger right| Rocket moves right
Tap canvas| Bullet fires
Bullet hits UFO| Explosion appears
Successful hit| Score +1
Bullet misses UFO| Bullet disappears
Tap Reset| Score returns to 0

📂 Project Structure

Rocket-vs-UFO/
│
└── rocket_vs_ufo.html

The complete game is contained in a single HTML file, including:

- HTML structure
- CSS styling
- JavaScript game logic

▶️ How to Run

1. Create a new file named:

rocket_vs_ufo.html

2. Copy the complete HTML code into the file.
3. Save the file.
4. Open the file using a web browser such as Chrome, Edge, or Firefox.
5. The game will start automatically.

📱 Controls

Mobile

- Drag your finger across the game area to move the rocket.
- Tap the game area to shoot.

Computer

- Move the mouse across the canvas to control the rocket.
- Click the canvas to shoot.

⚠️ Limitations

- No lives or health system.
- No game-over condition.
- UFO does not move continuously.
- Difficulty does not increase with the score.
- High scores are not saved after closing the browser.
- The game currently uses emoji-based rocket, UFO, and explosion graphics.

🚀 Future Improvements

The game can be improved by adding:

- ❤️ Lives and health system
- ⏱️ Timer or countdown
- 👽 Multiple UFOs
- 🚀 Different rocket designs
- 📈 Increasing difficulty
- 🏆 High-score storage using LocalStorage
- 💥 Better explosion animation
- 🎵 More sound effects
- 🌌 Animated space background
- 🎯 Different levels
- 🛡️ Power-ups and special weapons

📸 Screenshot

Add your game screenshot here:

![Rocket vs UFO Game](screenshot.png)

Place the screenshot file in the project folder and name it "screenshot.png".

📌 Project Information

Project Name: Rocket vs UFO
Platform: Web Browser
Technologies: HTML5, CSS3, JavaScript
Project Type: Mini Game / Mini Project
Development: Single-file web application

🏁 Result

The Rocket vs UFO game was successfully developed using HTML, CSS, and JavaScript. The player can control the rocket, shoot bullets at the UFO, detect collisions, display explosion effects, and maintain a running score. The game provides a simple and interactive browser-based gaming experience.
