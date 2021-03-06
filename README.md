# PittJumper: An ultra-simple 2D slider made with Pygame

## Overview:
PitJumper is an ultra-simple 2D-slider written in Python using Pygame, a set of python modules for media and game development.  The game was written with the intent to learn modern software development practices using version control, implement object-oriented design, and practice test-driven development strategies.  
## Game Features:
Despite its simplicity, PittJumper does have a moderate set of features that enhances gameplay and visual/audio characteristics.  These features are:

<ul>
<li>Game physics:</li>
<ul>
<li>User can move avatar left and right with respective left and right keys.</li>
<li>Collision detection for platform jumping and mobs.</li>
<li>User can make avatar jump using spacebar.</li>
<li>User can die by falling.
</ul>
<li>Robust soundtrack:</li>
<ul>
<li>In-game music track that fades out to pause menu.</li>
<li>Pause music track.</li>
<li>Game over chime.</li>
<li>Jump sound effects.</li>
</ul>
<li>Animations:</li>
<ul>
<li>Avatar animations respond to user input.</li>
<li>Avatar animated when stationary.</li>
<li>Enemy mobs are animated.</li>
</ul>
<li>Multiple frames:</li>
<ul>
<li>Game splash screen.</li>
<li>Game window.</li>
<li>Pause frame.</li>
<li>Game over frame.</li>
</ul>
<li>Gameplay:</li>
<ul>
<li>User can pause an active game.</li>
<li>User can view active game timer.</li>
<li>User's high score can be saved.</li>
</ul>

</ul>

    
## Running the Game:
This prompt assumes all dependencies have been installed on your system.  You will need the following for PitJumper to work correctly:

<ul>
<li>Python 3.6 or higher</li>
<li>Pygame</li>
</ul>
From the PittJumper directory on your screen, run the main.py file from the command line (bash in linux/MAC, or gitBash/command prompt in Windows):<br><br>

> <b>~$ python3 main.py</b>
## Understanding the Code:
PittJumper is executed from the main.py file from the main directory.  Main instantiates a new game object imported from game_class.py and calls the show_start_screen() method where it waits for user input.  When desired input is received, a new game begins with a call to new().  In addition to loading sprites, new() creates two timers and loads the music soundtrack.  The first timer is imported from the Pygame library and tracks total run time.  The second timer is an instance of the included Stopwatch class.  This timer sleeps while an active game is paused.  The difference between both timers returns overall game time which is used to calculate player score.  The soundtrack is managed using the built-in mixer from the Pygame module.  Finally, high scores are recorded in the highscore.txt file.  At the end of each game, the game object compares the current game score with data in highscore.txt.  If the current game score is higher, data in highscore.txt is overwritten which allows top scores to be stored offline.
## UML/Misc Diagrams:
![Class diagram](/classes_PittJumper.png)
![Relationships](/packages_PittJumper.png)
## Credits:
Chris Bradfield - Founder, KidsCanCode<br>
Artwork and Music from: OpenGameArt.org