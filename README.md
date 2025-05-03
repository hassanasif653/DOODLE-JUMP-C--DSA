📄 README – Doodle Jump Game (DSA Course Project)

🕹️ About the Game:
This is a C# Windows Forms Application of a Doodle Jump-style game with:

User Authentication:
Players must Register first, then Login before playing.

Game Features:
Character jumps on platforms.
Enemies and bullets.
Bonuses for power-ups.
Score tracking (score is shown at the top of the game screen).

🗂️ Forms:
1️⃣ Form1 – GameForm:

Main game window.
Shows the game area, player, platforms, enemies, bullets, and score at the top.

2️⃣ Form2 – LoginForm:

Users enter their username & password.
Successful login lets you play the game.

3️⃣ Form3 – RegisterForm:

New users can create an account.
Stores username & password data.

👥 User Management:
Class: User
Stores username and password.
Class: UserStore
Manages a list of users.
Handles:
Registering new users.
Checking login credentials.

✔️ DSA Concept:
The users can be stored in a List<User>, acting like a dynamic array.
You can also use a Dictionary<string, User> (for faster login lookup).

 Data Structures & Algorithms (DSA Concepts):
Dynamic Arrays (Lists):

List<Platform> to store all platforms.
List<Enemy> for enemies.
List<Bonus> for bonuses.
List<Bullet> for active bullets.

Collision Detection:
Iterates over game objects to check for collisions (looping over lists).

Queues or Stacks (Optional Idea):
A Queue<Bullet> could manage bullets, especially if there’s a firing rate cap.

Score Tracking:
A simple counter updated as the player jumps higher or defeats enemies.

Search (Login):
Linear search or use a Dictionary (Hash Table) for O(1) username lookups.

🚀 How It Works:
1️⃣ Register:

Open RegisterForm.
Enter username and password.
Data is stored in UserStore.

2️⃣ Login:

Open LoginForm.
Enter username and password.
If correct, open GameForm.

3️⃣ Play:

The game starts.
The player jumps on platforms and shoots enemies.
The score is shown at the top of the window.

🔑 Possible Enhancements:
Save user data to a file (like JSON or XML) for persistence.
Add a high-score table.
Use Binary Search Trees (BST) for a sorted leaderboard.

🛠️ Tech Used:
C# WinForms
visual studio
System.Drawing for graphics

Data Structures:
List
Dictionary

Basic Algorithms:

Collision Detection (Axis-Aligned Bounding Box - AABB)
•	Used to check for overlaps between rectangular objects such as platforms, bullets, and enemies.
•	Ensures accurate interaction by calculating positional deltas.
Physics Simulation:
•	Gravity and acceleration are applied to simulate realistic jumping and falling mechanics for the player and projectiles.
Platform Generation:
•	Platforms are generated with spacing rules and randomness to balance difficulty.
Monte Carlo Simulation:
•	Probabilistic spawning of bonuses and enemies based on predefined chances.
Object Pooling:
•	Prevents frequent memory allocation by reusing objects like bullets and enemies, improving performance.
Scoring System:
•	Points are awarded for actions such as jumping on platforms and defeating enemies. Scores are hashed using SHA-256 for security.


✅ To Run:
Open the project in Visual Studio.
Build and run.
Start by registering a new user.
Log in and enjoy the game!
