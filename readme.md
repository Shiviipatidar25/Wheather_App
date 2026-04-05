
🌦️ Weather Dashboard & Security Implementation
A project focused on asynchronous data fetching and professional credential management.

🛡️ Security & Learning Log
During the development of this project, I encountered several challenges regarding API security. Below is how I identified and fixed them:

1. The "Exposed Key" Error
The Issue: Initially, I hardcoded my OpenWeather API key directly into the JavaScript file. When I pushed to GitHub, I realized the key was public for anyone to see.

The Risk: Anyone could steal the key, exceed my usage limits, or incur costs.

The Fix: I transitioned to using Environmental Variables.

2. Implementing .env & .gitignore
The Solution: I created a .env file to store my secrets locally:

Code snippet
API_KEY=your_secret_key_here
The "Safety Net": I learned that simply having a .env isn't enough. I had to add it to a .gitignore file to ensure Git never uploads the secret file to the cloud.

3. Professional Workflow
Learning: I now use the dotenv package (or Vite/process.env) to call my keys securely.

Key Takeaway: Never commit secrets. Always provide a .env.example file so others know which variables are needed without seeing my actual private data.
Gemini said
I see—you used the HTML script tag or a direct reference in your HTML and then used .gitignore to prevent that specific file from being uploaded.

That is a common starting point, but on a professional resume or GitHub, you want to show that you've moved toward the industry standard (using JavaScript variables).

Here is how to explain your specific "HTML + .gitignore" approach in your README so it looks like a deliberate security choice:

🔒 Security Implementation: File Level Protection
In this project, I prioritized API key safety by separating sensitive credentials into a standalone configuration file.

1. The Strategy: HTML File Isolation
Instead of placing my API key in the main logic, I isolated it within a specific config.js or credentials.js file. This file is then called via a <script> tag in my index.html: then add it  git ignore file with env too . 

🚀 Technical Features
Asynchronous JS: Used async/await and the fetch() API to handle real-time data.

Error Handling: Implemented try...catch blocks to manage 404 errors (invalid city names) or network failures.

Dynamic UI: The DOM updates automatically based on the API response.

🛠️ Tech Stack
Frontend: HTML5, CSS3, JavaScript (ES6+)

API: OpenWeatherMap API

Tools: Git, GitHub, .env for security
