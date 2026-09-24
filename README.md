Rocket vs UFO 🚀👽
A single-screen Android app, built with MIT App Inventor, where a rocket at the bottom of the screen fires bullets at a UFO moving across the top — score a point every time you hit it.
How it works
The rocket starts centered near the bottom of the canvas, with the bullet and explosion sprites hidden
Drag anywhere on the canvas to slide the rocket left or right, following your finger's X position
Tap the rocket to fire — a bullet launches upward from just above the rocket, playing a shooting sound
If the bullet reaches the edge of the screen without hitting anything, it disappears
If the bullet collides with the UFO, an explosion plays at the UFO's position, a hit sound fires, and the score goes up by one
A timer briefly disables itself, then moves the UFO to a new random X position for the next round
Tap Reset to zero out the score at any time
Features
🚀 Drag-to-move rocket controlled by touch position on the canvas
🔫 Tap-to-shoot bullet that fires straight up from the rocket
👽 UFO that repositions to a random X position after being hit
💥 Explosion animation and sound effect on a successful hit
🔊 Separate sound effects for shooting and explosions
🏆 Running score counter with a one-tap Reset button
Tech Stack
Platform: MIT App Inventor (block-based, no native code)
Components: Canvas1, rocket, bullet, ufo, explosion, bulletsound, explosionsound, Clock1, score (label), resetbut (button)
How the Blocks Work
Event	Action
Screen1.Initialize	Centers the rocket horizontally at the bottom of the canvas, and hides the explosion and bullet sprites
Canvas1.Touched	Moves the rocket's X position to follow the touch point, offset by half the rocket's width so it centers under the finger
rocket.Touched	Moves the bullet to just above the rocket, plays the shoot sound, makes the bullet visible, and sends it upward (heading 90°, speed 30)
bullet.EdgeReached	Hides the bullet once it flies off the edge of the canvas with no hit
bullet.CollidedWith	Plays the explosion sound, moves the explosion sprite to the UFO's position, shows then hides the explosion, hides the bullet, increments the score, and re-enables the clock
Clock1.Timer	Disables itself, then moves the UFO to a new random X position within the canvas width, resetting the explosion's visibility
resetbut.Click	Resets the score label to 0
Example
Action	Result
Drag left/right	Rocket follows your finger
Tap rocket	Bullet fires upward
Bullet hits UFO	Explosion plays, score +1, UFO repositions
Bullet misses, reaches edge	Bullet disappears, ready to fire again
Tap Reset	Score returns to 0
Screenshot
�
The block workspace for the game — rocket movement, shooting, collision, and UFO respawn logic.
Limitations (v1.0)
No lives or game-over state — the UFO simply repositions after each hit
No increasing difficulty (UFO speed/frequency stays constant)
No animations beyond the built-in explosion visibility toggle
Score isn't persisted between sessions
Future Improvements
Add lives/health so the game can end
Increase UFO speed or spawn multiple UFOs as score climbs
Add a proper explosion animation and screen shake
Save high scores using TinyDB
Built as a mini project — MIT App Inventor, block-based development.
