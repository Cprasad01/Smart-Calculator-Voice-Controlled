# Smart-Calculator-Voice-Controlled:
Here is a detailed explanation of the code:

# Imported Libraries :

 The code begins by importing essential libraries that form the foundation of the calculator's functionality:

Tkinter:  This library provides the graphical user interface (GUI) components and event handling mechanisms for the calculator.

math: This library provides mathematical functions and constants required for calculations.

pygame.mixer: This library enables playing audio files, which is used for auditory feedback when pressing the microphone button.

speech_recognition: This library facilitates speech recognition, allowing the calculator to respond to voice commands.

threading: This library enables running tasks in parallel, which is utilized for handling speech recognition in a separate thread.

# Function Definitions :

The code defines several functions that handle specific aspects of the calculator's behavior:

click(): This function responds to button clicks. It takes the button value as input and performs the corresponding action, such as adding a digit, performing an operation, or clearing the entry field.

add(), sub(), mul(), div(), mod(), lcm(), and hcf(): These functions perform basic mathematical operations like addition, subtraction, multiplication, division, modulo, least common multiple, and highest common factor.

extraxt_from_text(): This function extracts numerical values from a text string, splitting it into words and converting each word that can be interpreted as a number into a float value.

audio(): This function handles speech recognition. It initializes the speech recognition engine, listens to the microphone, and recognizes spoken words. It then identifies mathematical operations in the recognized text and performs the corresponding calculations, updating the entry field with the result.

audio_thread(): This function creates a separate thread to handle speech recognition, allowing the calculator to remain responsive while waiting for voice commands.

# Main Calculator Logic

The main part of the code sets up the GUI layout and initializes the calculator's components. It creates the main window, adds logo and entry field widgets, and defines button widgets for numbers, operations, and special functions. It also creates a microphone button that triggers the speech recognition thread when clicked.

The mainloop() method starts the event loop, allowing the calculator to respond to user interactions, including button clicks and speech commands. When a button is clicked, the click() function is called to handle the corresponding action. When the microphone button is clicked, the audio_thread() function is called to start the speech recognition process.
