# Object Paint Web 🎨

Object Paint Web is a web-based paint application designed using an object-oriented model and various design patterns. It is implemented using Angular for the frontend and Java with the Spring Boot framework for the backend.

## Features ✨

- Free drawing
- Drawing shapes:
  - Circle
  - Ellipse
  - Square
  - Rectangle
  - Triangle
  - Line segment
- Edit drawn shapes:
  - Moving shapes by dragging
  - Resizing
  - Changing shapes' fill color
  - Changing shapes' border color
- Delete shapes
- Copy/paste
- Clear canvas
- Undo/Redo
- Save and load with chosen path in XML or JSON files.

## Design Patterns Applied 🎨

### Factory Design Pattern
We implemented a factory class responsible for creating the suitable shape using different classes of shapes that inherit from an abstract class (Shapes). Another class (Controller) acts as the client, holding all the information about the classes that will be created, and it uses the factory class.

### Prototype Design Pattern
We applied this pattern in the undo/redo functions where we needed to clone shapes from the redo stack to the undo stack and vice versa. This allowed us to make changes in one without affecting the other. Each class has implemented a clone function that overrides the clone function in the abstract parent class (Shapes).

## UML Class Diagram 📊

![UML Class Diagram](path/to/uml-class-diagram.png)
## How to Run 🏃‍♀️

1. Open any IDE for Java (IntelliJ, Eclipse, etc.).
2. Open the backend folder from File >> Open Folder.
3. If you don’t have JDK 19, download it or the IDE will prompt you to download it.
4. Run the main class.
5. Download Node.js.
6. From the terminal, install the Angular CLI globally with this command: `npm install -g @angular/cli`.
7. Open VS Code or any IDE that can open Angular.
8. Open the frontend folder from File >> Open Folder.
9. Open the terminal and run: `ng serve --open`.
10. Note: You might need this command: `npm install konva --save`.

## License 📄

This project is licensed under the [MIT License](LICENSE).

## Contact 📧

For any inquiries or suggestions, please contact us at [LinkedIn](https://www.linkedin.com/in/utkarsh-patidar-800081221/).

Thank you!! 👻💞
