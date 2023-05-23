# Quiz App

This is a simple quiz application that allows users to answer questions and receive a final score at the end. The code uses three modules: `question_model`, `data`, and `quiz_brain`.

## Installation

To use this code, you need to have Python 3.x installed on your system. No additional dependencies are required.

1. Download the source code from the repository.
2. Open a terminal or command prompt.
3. Navigate to the directory where the code is located.
4. Run the following command to execute the code:

   ```
   python quiz_app.py
   ```

## Usage

Upon running the code, a series of questions will be presented to the user. The user must provide their answer by typing it in the console and pressing Enter. After answering all the questions, the final score will be displayed.

## Code Overview

The code consists of the following components:

### `Question` Class (question_model.py)

This class represents a single question in the quiz. Each question has a text and an answer.

### `question_data` (data.py)

This module contains a list of dictionaries representing the questions and answers for the quiz. Each dictionary contains a `"text"` key for the question and an `"answer"` key for the correct answer.

### `QuizBrain` Class (quiz_brain.py)

The `QuizBrain` class manages the flow of the quiz. It keeps track of the current question number, the score, and the question bank. It also provides methods for getting the next question and checking the answer.

### Main Code

The main code performs the following steps:

1. Creates an empty list called `question_bank`.
2. Iterates over each dictionary in `question_data`.
3. Extracts the question text and answer from each dictionary.
4. Creates a new `Question` object using the extracted text and answer.
5. Appends the `Question` object to the `question_bank` list.
6. Creates a `QuizBrain` object, passing in the `question_bank`.
7. Enters a loop that continues as long as there are still questions in the quiz.
8. Calls the `next_question()` method of the `QuizBrain` object to display the next question and get the user's answer.
9. After the loop ends, displays a completion message and the final score.

## Customization

If you want to customize the quiz, you can modify the `question_data` list in the `data.py` module. Add or remove dictionaries representing the questions and answers as needed. Each dictionary should have a `"text"` key for the question and an `"answer"` key for the correct answer.

## Contributions

Contributions to this project are welcome. If you find any issues or would like to add new features, please open an issue or submit a pull request on the project repository.

## License

This code is released under the [MIT License](LICENSE). Feel free to use, modify, and distribute it as per the terms of the license.
