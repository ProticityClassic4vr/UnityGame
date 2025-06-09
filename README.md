Design Document (50%)

Player Experience (15%)

High Concept (5%)
This game is a platformer where a player guides a character through hazards, through levels, and collects objects on the way to finishing the level. This game’s main feature is its simple art style and the way it starts from the beginning whenever you win or lose. People playing the game are engaged, stimulated, and appreciated by overcoming easy but accurate settings.

Experience Goals (8%)
•	It has precise skills-based platforming and checkpoints that make you restart from the start.
•	In drama games, people face stressful challenges and feel happy when they are completed.
•	The design makes the game seem fun, childlike, and arcade-based.
•	Sound effects and collectible items give players a better experience and boost satisfaction.

Satisfaction of Player Needs (2%)
The game helps players gain competence by gradually making them better at moving and timing their efforts while getting all collectibles and crossing hazardous areas.

Game Mechanics (20%)
Player Controls and Movement (6%)
•	Controls and moving around the game are in need of improvement (6%)
•	MovementUtilizing Rigidbody2D, game objects can jump and move to the right or left.
•	Difficulties: When you fall off a platform, you have to start again and use good timing and space-awareness.
•	The style of the abstract avatar matches its neat and accurate motions.
•	You can use WASD or the Arrow Keys on the keyboard to play the game.
•	You have to be fast with your movements and watch your timing to overcome risks and challenges.
•	Players are expected to be familiar with classics from the Mario and Celeste universe.

Camera Design (2%)
•	You can notice the camera is either still or chases the player slightly in 2D mode.
•	It makes it easier for the player to keep track of danger zones and the goals while they play.

Good and Bad Things (5%)
•	It is good that collectibles are spawned at the beginning of the game.
•	DeathZone makes players start again.
•	The Drama Arc mode increases risk as you go, and the counter goes back to zero if you make an error.
•	Nervousness rises as the end is getting closer, but the player is still at risk of falling.
•	Jumping around the platforms needs a lot of care and attention.

Goals (3%)
•	The limelight pressures people to do their best, as they don’t want to fall again.
•	Jumping and movement are real-feeling in the game.
•	Collectibles increase your score and send players to look around before completing the level.

UI, Art & Audio Design (4%)
•	In the top part of the screen, a bold UI shows your progress.
•	Health system is not present (they are killed after falling once).
•	Blocky looks make the game easy to play and follow the fantasy vibe.
•	Vibration and sound make the game more enjoyable and satisfying.
•	Audio and the logic to restart really brings memorable highs and lows to the game.

Playtesting (15%)
Experience Goals:
•	The challenges were handled by creating concise gaps in the platforms.
•	The fact that the drama started again after being dead caused tension.
•	Having a minimalist art style made the game more interesting to play.
•	Sound and user interface elements helped the player meet the goals.

Positive Play Patterns
People were cautious before they jumped, showing they were working out the risks. Many players rushed back to play these locations again, which proved their attention span.

Negative Play Patterns
Some players couldn’t help falling out of the game because the control was so sensitive; others wanted there to be background music.

Improvements
Jumping between various platforms could be made smoother by changing the controls. Having background noise would increase how involved the player feels. It would be nice if the finish object looked different, and showing a “You Win” panel would explain that the quest is complete.

 Implementation Document
Feature	Completed	Related GameObject/Script
Sprites	Yes	Player, Finish, Collectibles
Tilemaps	Yes	implemented
Movement using Transform	Yes	(Used Rigidbody instead)
Movement using Rigidbody	Yes	Player, PlayerController.cs
Keyboard Controls using Input Asset	Yes	PlayerInput.cs
Gamepad Controls using Input Asset	Yes	Implemented
Trigger Colliders	Yes	Collectible, DeathZone
Physics Colliders	Yes	Player, Ground
Collision Events	Yes	GameManager.cs
Prefabs	Yes	Collectibles
Prefab - Dynamic Instantiation	No	(Unimplemented)
Object deactivation or destruction	Yes	Collectibles (destroy on collect)
UI layout	Yes	Canvas → ScoreText, RestartButton
UI updating	Yes	GameManager.cs
Camera - Basic	Yes	Main Camera
Camera - Cinemachine	No	(Unimplemented)
Audio - Looping	Yes	Implemented
Audio - Events	Yes	Collect and Win events

