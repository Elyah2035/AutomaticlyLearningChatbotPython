# Project Description: Chatbot with Knowledge Base

Repository: AutomaticlyLearningChatbotPython

Project Overview:
This project is a Python-based chatbot that interacts with users, answers questions, and learns new information to improve its knowledge base. It uses a knowledge base stored in a JSON file and the difflib library to find the closest matching question in the knowledge base for user queries. The chatbot can be a useful tool for providing information on a variety of topics.

# Features:

Load Knowledge Base: The chatbot loads its knowledge base from a JSON file at the beginning, which contains a collection of questions and answers.
Answering Questions: The chatbot continuously prompts the user for questions. It uses the get_close_matches function to find the closest matching question in the knowledge base.
Learning Capability: If the chatbot cannot find a match in its knowledge base, it asks the user to provide an answer. Users can type the answer, and the chatbot will learn from it by adding the new question-answer pair to the knowledge base.
Data Persistence: The chatbot can save the updated knowledge base to the JSON file, ensuring that the new information is retained for future interactions.
Exit Functionality: Users can exit the chatbot at any time by typing 'quit'.
Project Components:

load_knowledge_base(file_path: str): Function to read the knowledge base from a JSON file.

save_knowledge_base(file_path: str, data: dict): Function to write the updated knowledge base to a JSON file.

find_best_match(user_question: str, questions: list[str]) -> str | None: Function to find the closest matching question in the knowledge base.

get_answer_for_question(question: str, knowledge_base: dict) -> str | None: Function to retrieve the answer for a given question from the knowledge base.

chatbot(): The main function that runs the chatbot and handles user interactions. It loads the knowledge base, interacts with the user, and manages learning and data persistence.

# How to Use:
Clone the repository to your local machine. 
Install the required libraries, mainly json and difflib, if not already installed. 
Run the chatbot() function in the Python script. 
Start asking questions or type 'quit' to exit the chatbot. 
When the chatbot doesn't know the answer to a question, you can teach it by providing an answer. The chatbot will learn and store the new information. 

# Example:

You: What is the capital of France?

Bot: I don't know the answer. Can you teach me?

Type the answer or 'skip' to skip: Paris

Bot: Thank you! I've learned something new.


# Contribution:
Contributions to this project, such as improvements in question-answering accuracy, user interface enhancements, or other features, are welcome. You can fork the repository, make your changes, and create a pull request.
