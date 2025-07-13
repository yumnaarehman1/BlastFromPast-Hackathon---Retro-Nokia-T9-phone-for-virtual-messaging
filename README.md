# BlastFromPast-Hackathon---SMS Terminal : Retro-Nokia-T9-phone-for-virtual-messaging

SMS Terminal is a retro-style web application that simulates the T9 typing experience of classic Nokia phones. Users can type messages using a virtual numeric keypad and send them as SMS using the Twilio API.

This project was built as part of the OSDHACK 2025 hackathon under the theme "Blast from the Past", where the goal was to reimagine retro technologies using modern tools.

# Features
T9 keypad interface implemented in JavaScript

SMS sending via Twilio API (trial account supported)

Live message preview display

Simple, clean UI inspired by early mobile interfaces

Fully open-source and easy to customize

Technologies Used
HTML, CSS, JavaScript

Node.js with Express.js

Twilio API for SMS functionality

Dotenv for environment variable handling

# How It Works
User types a message using the numeric keypad.

The app maps key presses to T9 characters using timeout-based cycling.

Upon pressing "Send", the message and recipient number are sent to the backend.

The Express server uses Twilio to send the SMS to the provided phone number.

# Requirements
A verified Twilio account (trial or paid)

A verified recipient phone number (for trial accounts)

Node.js and npm installed locally

Setup Instructions
Clone the repository.

Run npm install to install dependencies.

Create a .env file and add the following:
 
TWILIO_SID=your_account_sid
TWILIO_AUTH=your_auth_token
TWILIO_PHONE=your_twilio_trial_number

Run the server using:
 
node server.js
Open index.html in your browser and test the application.

# Limitations
Twilio trial accounts can only send SMS to verified numbers.

This app does not support predictive T9 dictionaries (only multi-tap style).
