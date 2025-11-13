Flappy Bird Game (Java)

A simple Flappy Bird clone built in Java using Java Swing for graphics and OOP concepts for game mechanics.
This project demonstrates object-oriented design, event handling, and basic physics for game development.

🎮 Features

Flappy Bird style gameplay with gravity and jump mechanics

Obstacle generation (pipes) with collision detection

Score tracking

Responsive keyboard input using Java KeyListener

Lightweight and runs without external libraries

📂 Project Structure
├── App.java          # Entry point of the application
├── FlappyBird.java   # Main game logic, rendering, and physics
├── KeyListner.java   # Handles user keyboard inputs (jump / restart)

🚀 How to Run

Clone the repository:

git clone https://github.com/your-username/flappy-bird-java.git
cd flappy-bird-java


Compile the Java files:

javac App.java FlappyBird.java KeyListner.java


Run the game:

java App

🖼️ Gameplay Preview

(You can add a screenshot or GIF of the game here once available.)

🛠️ Tech Stack

Java (Core, OOP concepts)

Swing (for GUI & graphics)

📘 Learning Highlights

Implementing physics (gravity & velocity) in 2D games

Using KeyListener for real-time input

Object-Oriented Programming principles in game design

Managing game loops and repaint cycles in Java Swing

🤝 Contributing

Feel free to fork this repository, raise issues, and submit pull requests. Contributions are welcome!

📄 License

This project is licensed under the MIT License – you’re free to use, modify, and distribute it.

👉 Do you want me to also add code snippets inside README (like how KeyListner handles jump input) to make it more illustrative, or keep it short and clean?

You said:
add code snippets inside readme
ChatGPT said:

Perfect 👍 Adding code snippets inside the README will make it more illustrative for anyone visiting your GitHub repo. I’ll keep them short and explanatory so that users get a feel of how the game works without reading the full source code.

Here’s the updated README.md with code snippets:

Flappy Bird Game (Java)

A simple Flappy Bird clone built in Java using Java Swing for graphics and OOP concepts for game mechanics.
This project demonstrates object-oriented design, event handling, and basic physics for game development.

🎮 Features

Flappy Bird style gameplay with gravity and jump mechanics

Obstacle generation (pipes) with collision detection

Score tracking

Responsive keyboard input using Java KeyListener

Lightweight and runs without external libraries

📂 Project Structure
├── App.java          # Entry point of the application
├── FlappyBird.java   # Main game logic, rendering, and physics
├── KeyListner.java   # Handles user keyboard inputs (jump / restart)

🚀 How to Run

Clone the repository:

git clone https://github.com/your-username/flappy-bird-java.git
cd flappy-bird-java


Compile the Java files:

javac App.java FlappyBird.java KeyListner.java


Run the game:

java App

🖥️ Example Code Snippets
🔹 App.java – Entry Point
public class App {
    public static void main(String[] args) {
        // Start the game by creating a new FlappyBird instance
        new FlappyBird();
    }
}


The game starts by running the FlappyBird class, which sets up the game window and loop.

🔹 FlappyBird.java – Game Loop & Physics
// Gravity & velocity logic
if (birdY + velocity < frameHeight) {
    velocity += gravity;
    birdY += velocity;
}

// Pipe movement
for (Rectangle pipe : pipes) {
    pipe.x -= speed;
}


Handles gravity, jump physics, and pipe movement inside the main game loop.

🔹 KeyListner.java – Player Controls
@Override
public void keyPressed(KeyEvent e) {
    if (e.getKeyCode() == KeyEvent.VK_SPACE) {
        velocity = -10; // Bird jumps when SPACE is pressed
    }
}


The spacebar lets the bird jump by applying a negative velocity.


🛠️ Tech Stack

Java (Core, OOP concepts)

Swing (for GUI & graphics)

📘 Learning Highlights

Implementing physics (gravity & velocity) in 2D games

Using KeyListener for real-time input

Object-Oriented Programming principles in game design

Managing game loops and repaint cycles in Java Swing

🤝 Contributing

Feel free to fork this repository, raise issues, and submit pull requests. Contributions are welcome!
