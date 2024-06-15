Drawing App with React

This project is a simple drawing application built using React, leveraging functional components, React Hooks, HTML Canvas, and JavaScript ES6 features.

Prerequisites
Before running this project, ensure you have the following prerequisites installed:

React: Make sure you have Node.js and npm installed. You can install React using:

npx create-react-app drawing-app
cd drawing-app

Functional Components: Familiarity with React functional components is recommended.

React Hooks: Understanding of React Hooks (useState, useEffect, etc.) is required.

HTML Canvas: Basic knowledge of HTML Canvas element and drawing operations.

JavaScript ES6: Comfortable with modern JavaScript ES6 syntax and concepts.

Approach

In this application, we implement three main functions to enable drawing functionality:

startDrawing(): This function starts the drawing process when the mouse button is pressed down. It captures the initial coordinates (startX, startY) and toggles the isDrawing state to true.

draw(): The draw() function is called when the mouse is moved while drawing (isDrawing is true). It draws a stroke using the current coordinates (x, y) on the canvas context.

endDrawing(): When the mouse button is released, endDrawing() is executed. It closes the current drawing path on the canvas context and sets isDrawing to false.

Implementation Details
Canvas Setup: The HTML <canvas> element is used to render the drawing area. We obtain its context using canvasRef.current.getContext('2d').

Event Listeners: Event listeners (mousedown, mousemove, mouseup, mouseleave) are attached to the canvas to trigger the drawing functions based on user interaction.

State Management: React Hooks (useState) are used to manage state variables such as isDrawing, startX, startY, x, and y.

Usage

Clone the repository:

git clone <repository_url>

cd drawing-app

Install dependencies:

npm install

Start the development server:

npm start

Open http://localhost:3000 in your browser.

Use the mouse to draw on the canvas. Click and drag to draw strokes, release the mouse button to stop drawing.
