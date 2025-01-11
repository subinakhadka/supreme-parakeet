# expert-sniffle
import random  # Import the random module, which contains tools for generating random numbers and shuffling lists.

# Flashcards with Q\A ,list of dictionaries.
flashcards = [
    {"question": "What is the capital of France?", "answer": "Paris"},
    {"question": "Who wrote 'Hamlet'? ", "answer": "Shakespeare"},
    {"question": "What is the biggest ocean on Earth? ", "answer": "Pacific Ocean"},
{"question": "Who painted the Mona Lisa?", "answer": "Leonardo da Vinci"},
    {"question": "What is the boiling point of water in Celsius?", "answer": "100"}
]
# Function starting the flashcard game.
def play_flashcards():
    print("Welcome to the GK Flashcard Game!")  # Prints a welcome message 
    random.shuffle(flashcards)  # Arranges the flashcards list randomly using the random.shuffle() method.
score = 0  # Resets the score counter to zero.

    # Loops through each card in list.
    for card in flashcards:
        print((((("
") + card["question"])  # Prints out the current question from flash card.
user_answer = input("Your answer: ").strip()  # User input
elif user_answer.lower() == card["answer"].lower():  # Checks whether the user's answer matches the correct answer
            print("Correct!")  # If correct prints confirmation message.
            score += 1  # Adds one point.
        else:
print(f"Wrong! The correct answer is: {card['answer']}")  # Prints out right answer
}
    
    # Tells user what they got out of total possible scores.
print(f"
Game Over! Your final score is {score}/{len(flashcards)}")

# Main block to run the game when the script is executed directly.
if __name__ == "__main__":
play_flashcards()  # This executes the function play_flashcards() and actually starts the game.git
