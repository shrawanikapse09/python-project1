def ask_question(question, options, correct_answer):
    print(question)
    for i, option in enumerate(options, 1):
        print(f"{i}. {option}")
    
    while True:
        try:
            answer = int(input("Your answer (1-4): "))
            if 1 <= answer <= 4:
                break
            else:
                print("Invalid input. Please enter a number between 1 and 4.")
        except ValueError:
            print("Invalid input. Please enter a number between 1 and 4.")
    
    if options[answer - 1] == correct_answer:
        print("Correct!")
        return True
    else:
        print(f"Incorrect. The correct answer is: {correct_answer}")
        return False

def quiz():
    questions = [
        {
            "question": "which of the following is capital of India?",
            "options": ["mumbai", " New Delhi", "Chennai", "Banglore"],
            "answer": " New Delhi"
        },
        {
            "question": "which of the following is national animal of India?",
            "options": ["Tiger", "Lion", "Cow", "Elephant"],
            "answer": "Tiger"
        },
        {
            "question": "how many states are there in India?",
            "options": ["30", "28", "31", "32"],
            "answer": "28"
        }
    ]
    
    score = 0
    
    for q in questions:
        if ask_question(q["question"], q["options"], q["answer"]):
            score += 1
    
    print(f"\nYour final score is: {score}/{len(questions)}")

if __name__ == "__main__":
    quiz()
