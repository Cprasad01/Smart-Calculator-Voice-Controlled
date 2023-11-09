# Smart-Calculator-Voice-Controlled

 The provided code outlines a smart calculator capable of voice-controlled operations, implemented using Python programming language. It utilizes the SpeechRecognition and Pygame libraries to enable speech recognition and graphical user interface elements, respectively.

The code structure involves defining functions for speech recognition, mathematical calculations, and displaying results. The main function orchestrates these components to create a seamless user experience.

The speech recognition function employs the SpeechRecognition library to capture and interpret spoken commands. It converts the captured audio into text and extracts the numerical values and operators.

The mathematical calculations function handles the actual computations, taking the extracted numerical values and operators from the speech recognition function. It performs the corresponding arithmetic operations and returns the result.

The display results function utilizes the Pygame library to create a graphical interface and display the calculated result. It generates a visually appealing output that is easily understood by the user.

The main function integrates these functions to achieve the overall functionality of the smart calculator. It starts by initializing the speech recognizer and Pygame modules. Then, it enters a continuous loop that listens for voice commands.

Upon receiving a voice command, the speech recognition function is activated to extract the numerical values and operators. These extracted values are then passed to the mathematical calculations function to perform the necessary computations.

The resulting calculation is finally passed to the display results function, which generates a visual representation of the outcome on the user's screen. This completes the cycle of voice command interpretation, calculation, and result presentation.
