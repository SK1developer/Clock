# Clock
 project -Clock
Analog Clock using HTML, CSS, and JavaScript
This project is a dynamic analog clock that visually represents real-time hours, minutes, and seconds using a modern, stylish design. Built using HTML, CSS, and JavaScript, the clock offers a smooth and interactive experience. The project is simple yet effective, providing a great way to understand DOM manipulation, CSS animations, and JavaScript's Date object.

Key Features:
Real-Time Clock Display

The clock updates every second to display the exact time.
The hour, minute, and second hands move smoothly in synchronization with the actual time.
Minimalist and Modern UI

The clock has a dark-themed background with a circular design.
The hour, minute, and second hands have different colors for easy distinction.
The numbers are arranged in a classic clock style with a rotated effect.
Custom Styling using CSS

The clock face is designed with a shadow effect to give a realistic appearance.
The hands of the clock are animated with rotational transformations.
CSS variables are used for better flexibility in design.
JavaScript Time Calculation

JavaScript retrieves the current time and calculates the appropriate rotation for the hands.
The hour hand moves 30 degrees per hour, the minute hand 6 degrees per minute, and the second hand 6 degrees per second.
The setInterval() function ensures smooth movement.
Social Media Branding (Code.WithChiku)

The clock includes a branding link with an Instagram icon that redirects users to the code.withchiku Instagram page.
Breakdown of the Code Files
1. index.html (HTML Structure)
This file provides the structure of the web page. It includes:

A container div to hold the clock.
A branding section with an Instagram link.
A clock div that contains:
A central rotating mechanism for hour, minute, and second hands.
Numbered hour markers placed dynamically.
A script tag linking the script.js file.
2. styles.css (Styling)
General Styling: The page uses flexbox to center the clock.
Clock Face: The clock has a circular design with a dark theme and a subtle border.
Hands Styling:
Each hand has a different color (rgb values).
transform: rotate() is used to position the hands correctly.
Number Markers:
The numbers (1-12) are placed dynamically using rotate(calc(30deg * var(--1))) for correct alignment.
3. script.js (JavaScript Functionality)
JavaScript dynamically updates the rotation of the clock hands.
displayTime() function:
Retrieves the current hour, minute, and second.
Calculates the angle of rotation for each hand.
Applies the rotation using transform: rotate(deg).
The function runs every second using setInterval(displayTime, 1000).
