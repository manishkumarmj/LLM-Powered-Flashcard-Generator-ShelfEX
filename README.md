# LLM-Powered-Flashcard-Generator-ShelfEX
# Anki Flashcards Creator from PDF  ( being honest i have taken help from a https://www.youtube.com/watch?v=t08xpI2JNyA) totaly honest with  you all 
not

------------------------------------------------------------ 
#Phase 1: Complete Summary

My project, the Anki Flashcards Creator, is a Python script designed to automate flashcard generation from PDFs. I used PyPDF2 (now part of pypdf) to extract text and openai to interact with AI models like GPT-4.1 ( git market place for free for few days )  for Q&A generation. The process involves os for path management and tiktoken for token handling. I built it within a conda virtual environment (anki_cards) to manage dependencies. The script outputs .txt files for Anki import. We overcame significant setup and library versioning challenges to make it functional.
-------------------------------------------------------------------------------------------------
# Setup and Installation
1. initial Setup: Started by installing Conda and initializing PowerShell, which was crucial for environment management.
2. Environment Creation: Created a dedicated anki_cards Conda environment to isolate project dependencies effectively.
3. Package Installation: Installed core libraries like PyPDF2, openai, and tiktoken using pip within my activated Conda environment.
4. VS Code Configuration: Critically, configured VS Code's Python interpreter and Jupyter kernel to correctly use my anki_cards environment.
5.API Key Setup: Secured my OpenAI API key by setting it as an environment variable, then retrieving it in the script.
6. PDF Reading: My script reads the target PDF using PyPDF2, extracting all available text content.
7. Text Chunking: The extracted text is divided into smaller sections to fit within the OpenAI model's token limits.
8. AI Flashcard Generation: Each text chunk is sent to OpenAI (e.g., GPT-3.5 Turbo) via the openai library's new API.
9. Output Saving: Generated question-answer pairs are then compiled and saved to a flashcards.txt file.
10. Anki Import Ready: The final text file is formatted to be easily imported into the Anki flashcard application.
--------------------------------------------------------------------------------------------------
# My Key Takeaways & Lessons Learned
1.  Developing this project offered valuable insights beyond just coding:
2.  Project Isolation: I learned local dependencies are crucial for clean, conflict-free project environments.
3.  Precise Package Management: Mastering pip was key, ensuring installations went into the activated Conda environment.
4.  Virtual Environment Power: Conda environments provided essential isolation for specific project dependencies.
5.  Consistent Setup: Configuring my IDE's Python interpreter and kernel correctly proved consistently vital.
6.  API Cost Awareness: I realized OpenAI API calls are not free, monitoring usage is important.
7.  Iterative Problem Solving: Solving one issue often led to another, teaching me systematic debugging.
