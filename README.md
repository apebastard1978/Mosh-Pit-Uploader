Mosh Pit Trivia - Content Management System (CMS)
This is a web-based uploader and content management tool for the "Mosh Pit Trivia" game. It provides a user-friendly interface to add, manage, edit, and delete trivia questions stored in a Firebase Firestore database.

Features
This tool provides a complete solution for managing the game's content with three distinct modes:

Manage Questions:

View all questions currently in the database in a clean, paginated list.

Search for specific questions by keyword.

Filter questions by Category (Bulk, Curated, Picture) or by Season.

Edit any existing question with a single click, which populates the manual entry form.

Delete questions from the database (with confirmation).

Manual Entry:

A full form for adding new questions or saving edits to existing ones.

Includes fields for Category, Season, Topic, Question Text, Image URL, and four answers.

Radio buttons for easy selection of the correct answer.

Smart logic to automatically suggest the "Picture" category if an Image URL is entered.

AI Generator:

Leverages the Gemini API to automatically generate new trivia questions based on simple facts.

Includes templates for different question types:

Album Release Year

Song from Lyric

Song on Album

Automatically populates the "Manual Entry" form with the AI-generated content, allowing for review and editing before saving.

Bulk JSON Upload:

A simple text area for pasting the contents of an entire questions.json file.

Allows for adding a large number of pre-written questions to the database in a single batch operation.

Setup
To run this tool locally, you will need:

A Firebase Project: This tool is designed to connect to your game's Firebase project.

VS Code with Live Server: The Live Server extension is required to run the file locally and avoid browser security errors.

A Gemini API Key: For the AI Generator feature. You can get a free key from Google AI Studio.

Configuration
Before running the tool, you must add your credentials to the index.html (or uploader.html) file:

Firebase Credentials: Open the file and find the firebaseConfig object in the <script> section. Paste your configuration object from your Firebase project settings.

Gemini API Key: In the same script, find the apiKey constant inside the generateButton.addEventListener function and paste your Gemini API key.

How to Use
Open your project folder in VS Code.

Right-click on the index.html (or uploader.html) file and select "Open with Live Server".

The tool will open in your browser, ready to use.

Use the tabs at the top to switch between managing existing questions, adding new ones manually, or generating them with AI.
