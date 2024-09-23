# Pong-Game
The Pong game is a classic arcade-style game that simulates table tennis. The objective is for players (or a player vs. computer) to bounce a ball back and forth using paddles without letting the ball go past them. This project serves as an excellent introduction to game development and graphical programming in Java using the Swing framework.

**About**

*Game Mechanics:*
Pong is a simple two-dimensional sports game that simulates table tennis. Players control paddles to hit a ball back and forth.
The goal is to score points by making the opponent miss the ball.

*Graphics and User Interface:*
The game is built using Java’s AWT and Swing libraries, which provide the tools for creating a graphical user interface.
The JFrame class is used to create the main game window, while JPanel is used for rendering the game components.

*Game Loop:*
The game runs in a continuous loop (the run method), which updates game state, checks for collisions, and repaints the screen at a fixed rate (60 ticks per second).

*Event Handling:*
User inputs (keyboard presses) are handled through key listeners, allowing players to control the paddles.

**OOP Concepts Used**

*Classes and Objects:*
Each component of the game (paddles, ball, score) is represented as a class. For instance, Paddle, Ball, and Score are distinct classes that encapsulate their own attributes and behaviors.
Objects of these classes are created and manipulated throughout the game.

*Encapsulation:*
Each class hides its internal state and exposes methods to interact with it. For example, the Paddle class manages its position and movement without exposing its internal details directly.
Attributes like x, y, width, and height are private in the parent Rectangle class, ensuring they can't be accessed directly.

*Inheritance:*
The Paddle, Ball, and Score classes extend the Rectangle class, inheriting its properties and methods. This allows them to leverage existing functionality for positioning and collision detection.

*Polymorphism:*
The game uses polymorphism through method overriding. For example, each object implements its own draw method to render itself on the screen differently.

*Abstraction:*
The game abstracts complex behaviors into simple methods. For instance, the move and draw methods encapsulate the logic for updating positions and rendering the paddles and ball.

*Composition:*
The GamePanel class is composed of multiple objects, including two Paddle objects, a Ball, and a Score object. This composition allows GamePanel to manage all game elements in one place.
