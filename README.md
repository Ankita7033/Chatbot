# Chatbot

# Creative Prompt Generator Chatbot
This project implements an intelligent chatbot that generates creative prompts based on user input. The chatbot allows users to choose a genre, provides creative prompts, and stores the user's history and favorite prompts for future use. The prompts can be generated for different types of content such as story, quote, setting, dialogue, and more.

The chatbot is powered by the Gemini API to generate creative prompts based on text or images that the user provides.

Features:
1.Text-to-Image Prompts: The chatbot generates creative prompts based on user input text or image.
2.Genre Selection: Users can choose from various genres like horror, sci-fi, fantasy, etc., to tailor the prompts.
3.Prompt History: Users can view their previous prompts, which are stored for reference.
4.Favorite Prompts: Users can mark prompts as favorites for easy access later.
5.Integration with Gemini API: The chatbot uses the Gemini API key to generate unique prompts based on the input.

# Project Structure:
- bot.py                           # Main chatbot script
- prompts_db.json                  # Database for storing user prompt history and favorite prompts
- requirements.txt                 # List of dependencies
- README.md                        # This file
- LICENSE                          # Project license

# Installation:
   1. Clone the repository:
    git clone https://github.com/YourUsername/Creative-Prompt-Generator-Chatbot.git
    2.Install dependencies: Create a virtual environment (optional but recommended):
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    Install the required Python packages:
    pip install -r requirements.txt

  3.Set up Gemini API Key:
  Obtain your Gemini API Key from the official Gemini API provider.
  Add your API key to the environment variables or directly in the script.

 4. Run the chatbot:
  Start the chatbot by running:
  python bot.py

# How It Works:
1.Start the Chatbot: The chatbot will greet the user and prompt for input to generate a creative prompt. It can handle both text and image inputs.

2.Choose Genre: The user can select a genre, such as horror, sci-fi, or fantasy, to generate prompts tailored to the selected genre.

3.Generate Prompt: The chatbot will use the Gemini API to generate a creative prompt based on the user's input (text or image). The user will be shown a variety of prompts to choose from.

4.Prompt History: The chatbot will store the user's previously generated prompts in a local database (prompts_db.json). Users can view their history and revisit any previous prompts.

5.Save Favorite Prompts: Users can mark any prompt as a favorite, and these will be stored separately in the database for quick access later.

# Example Interaction:
Welcome to the Creative Prompt Generator Chatbot!
------------------------------------------------
Choose a genre:
1. Horror
2. Sci-Fi
3. Fantasy
4. Romance
Enter your choice (1/2/3/4): 2

Please enter a description or upload an image to generate a prompt:
> A futuristic city with towering skyscrapers and flying cars.

Fetching prompts...
Prompt 1: "A journey to a distant galaxy where humanity has established new colonies."
Prompt 2: "The discovery of a hidden alien artifact deep beneath the city streets."
Prompt 3: "A rebellion against a totalitarian government in a high-tech world."

Enter the number of your chosen prompt: 2

Your selected prompt: "The discovery of a hidden alien artifact deep beneath the city streets."

Would you like to:
1. Save as Favorite
2. View Prompt History
3. Exit
Enter your choice (1/2/3): 1
Prompt saved as Favorite!

# Database Structure (prompts_db.json):
{
  "history": [
     "A journey to a distant galaxy where humanity has established new colonies.",
    "The discovery of a hidden alien artifact deep beneath the city streets."
  ],
  "favorites": [
    "The discovery of a hidden alien artifact deep beneath the city streets."
  ]
}

# API Usage:
The chatbot uses the Gemini API to generate creative prompts. The API key is required for authentication. To ensure smooth API usage, please refer to the Gemini API documentation for rate limits and query parameters.


