print("====================================")
print("       PYTHON TUTORIAL SYSTEM      ")
print("====================================")
print("Welcome to Python Tutorial!")
print("Learn Python through lessons and activities.")

while True:
    
    print("\n========== LESSON CHOICES ==========")
    print("1. Prelim Lessons")
    print("2. Midterm Lessons")
    print("3. Finals Lessons")
    print("4. Exit")

    choice = input("\nChoose your lesson: ")
    chapter = "0"

    if choice == "1":
        print("\n========== PRELIM CHAPTERS ==========")
        print("1. Introduction to Programming")
        print("2. Python Basic Syntax")
        print("3. Arithmetic Operators and Expressions")
        print("4. Basic Input and Output")

        chapter_choice = input("\nChoose a chapter: ")

        if chapter_choice == "1":
            chapter = "1"
        elif chapter_choice == "2":
            chapter = "2"
        elif chapter_choice == "3":
            chapter = "3"
        elif chapter_choice == "4":
            chapter = "4"
        else:
            print("Invalid chapter choice.")

    elif choice == "2":
        print("\n========== MIDTERM CHAPTERS ==========")
        print("5. Conditional Statements")
        print("6. Logical Operators")

        chapter_choice = input("\nChoose a chapter: ")

        if chapter_choice == "5":
            chapter = "5"
        elif chapter_choice == "6":
            chapter = "6"
        else:
            print("Invalid chapter choice.")

    elif choice == "3":
        print("\n========== FINALS CHAPTERS ==========")
        print("7. Introduction to Iteration and Loops")

        chapter_choice = input("\nChoose a chapter: ")

        if chapter_choice == "7":
            chapter = "7"
        else:
            print("Invalid chapter choice.")

    elif choice == "4":
        print("\nThank you for using Python Tutorial!")
        break

    else:
        print("\nInvalid choice. Please try again.")

    if chapter != "0":

        # CHAPTER 1
        if chapter == "1":
            print("""
         ================= CHAPTER 1 =================
         INTRODUCTION TO PROGRAMMING

         Programming is the process of giving instructions
         to a computer to perform a specific task.

         Python is a programming language that is easy to
         read and understand. It is used to create programs,
         solve problems, and automate tasks.

         Example:
         print("Hello, World!")

         The print() function displays a message on the screen.
         """)

            question1 = "What is programming?"
            option1 = "A. Playing computer games"
            option2 = "B. Giving instructions to a computer"
            option3 = "C. Browsing the internet"
            correct1 = "B"

            question2 = "Which programming language are we learning?"
            option4 = "A. Java"
            option5 = "B. C++"
            option6 = "C. Python"
            correct2 = "C"

            question3 = "What is the purpose of a program?"
            option7 = "A. To perform a specific task"
            option8 = "B. To turn off the computer"
            option9 = "C. To delete all files"
            correct3 = "A"

        # CHAPTER 2
        elif chapter == "2":
            print("""
         ================= CHAPTER 2 ====================
         PYTHON BASIC SYNTAX

         Syntax refers to the rules used in writing Python code.

         PRINTING OUTPUT:
         The print() function displays text or values.

         Example:
         print("Hello!")

         COMMENTS:
         Comments are notes in the code. They are ignored
         when the program runs. Use # to write a comment.

         Example:
         # This is a comment

         VARIABLES AND DATA TYPES:
         Variables store information that can be used later.

         Examples:
         name = "Alex"
         age = 18
         grade = 95.5

         Common data types:
         str - Text
         int - Whole numbers
         float - Decimal numbers
         bool - True or False
         """)

            question1 = "Which function displays output?"
            option1 = "A. input()"
            option2 = "B. print()"
            option3 = "C. type()"
            correct1 = "B"

            question2 = "Which symbol is used for comments?"
            option4 = "A. #"
            option5 = "B. @"
            option6 = "C. $"
            correct2 = "A"

            question3 = "Which data type is used for decimal numbers?"
            option7 = "A. int"
            option8 = "B. str"
            option9 = "C. float"
            correct3 = "C"

        # CHAPTER 3
        elif chapter == "3":
            print("""
         ================= CHAPTER 3 =================
         ARITHMETIC OPERATORS AND EXPRESSIONS

         Arithmetic operators are used to perform
         mathematical operations in Python.

         Common operators:

         +  Addition
         -  Subtraction
         *  Multiplication
         /  Division
         %  Modulus
         ** Exponent
         // Floor Division

         Example:
         x = 10
         y = 5

         print(x + y)
         print(x * y)

         EXPRESSIONS IN PYTHON:
         Expressions are combinations of values and operators.

         PEMDAS - is used to determine the order of operations:
         Parentheses, Exponents, Multiplication, Division,
         Addition, and Subtraction.
         """)

            question1 = "Which operator is used for multiplication?"
            option1 = "A. +"
            option2 = "B. *"
            option3 = "C. /"
            correct1 = "B"

            question2 = "What is the result of 10 + 5 * 2?"
            option4 = "A. 30"
            option5 = "B. 20"
            option6 = "C. 25"
            correct2 = "B"

            question3 = "Which operator is used for exponent?"
            option7 = "A. **"
            option8 = "B. //"
            option9 = "C. %"
            correct3 = "A"

        # CHAPTER 4
        elif chapter == "4":
            print("""
         ================= CHAPTER 4 =================
         BASIC INPUT AND OUTPUT IN PYTHON

         INPUT:
         The input() function allows the user to enter
         information into the program.

         Example:
         name = input("Enter your name: ")

         FORMATTING OUTPUT:
         An f-string allows us to display variables
         together with text.

         Example:
         name = "Alex"
         print(f"Hello, {name}!")

         TYPE CONVERSION:
         Input values are treated as text by default.
         We can convert them into other data types.

         int() - Converts a value to a whole number
         float() - Converts a value to a decimal number

         Example:
         age = int(input("Enter your age: "))
         """)

            question1 = "Which function accepts user input?"
            option1 = "A. print()"
            option2 = "B. input()"
            option3 = "C. float()"
            correct1 = "B"

            question2 = "Which function converts input to a whole number?"
            option4 = "A. int()"
            option5 = "B. str()"
            option6 = "C. print()"
            correct2 = "A"

            question3 = "What is used to format output with variables?"
            option7 = "A. Comment"
            option8 = "B. While loop"
            option9 = "C. f-string"
            correct3 = "C"

        # CHAPTER 5
        elif chapter == "5":
            print("""
         ================= CHAPTER 5 =================
         CONDITIONAL STATEMENTS

         Conditional statements allow a program to make
         decisions based on certain conditions.

         RELATIONAL OPERATORS:
         These operators compare two values.

         >  Greater than
         <  Less than
         == Equal to
         != Not equal to
         >= Greater than or equal to
         <= Less than or equal to

         IF STATEMENT:
         Runs a block of code when a condition is True.

         IF-ELSE STATEMENT:
         Chooses between two possible actions.

         IF-ELIF-ELSE STATEMENT:
         Checks multiple conditions.

         NESTED CONDITION:
         An if statement placed inside another if statement.

         Example:
         age = 18

         if age >= 18:
             print("Adult")
         else:
             print("Minor")
         """)

            question1 = "Which statement is used to make decisions?"
            option1 = "A. if"
            option2 = "B. print"
            option3 = "C. input"
            correct1 = "A"

            question2 = "What does the == operator mean?"
            option4 = "A. Greater than"
            option5 = "B. Equal to"
            option6 = "C. Not equal to"
            correct2 = "B"

            question3 = "Which statement checks another condition?"
            option7 = "A. break"
            option8 = "B. while"
            option9 = "C. elif"
            correct3 = "C"

        # CHAPTER 6
        elif chapter == "6":
            print("""
         ================= CHAPTER 6 =================
         LOGICAL OPERATORS

         Logical operators are used to combine or
         reverse conditions in Python.

         AND:
         Returns True when both conditions are True.

         OR:
         Returns True when at least one condition is True.

         NOT:
         Reverses the result of a condition.

         Examples:
         age = 18
         has_id = True

         print(age >= 18 and has_id)
         print(age >= 18 or has_id)
         print(not has_id)

         Logical operators help programs check
         more than one condition.
         """)

            question1 = "Which operator requires both conditions to be True?"
            option1 = "A. or"
            option2 = "B. and"
            option3 = "C. not"
            correct1 = "B"

            question2 = "Which operator is True if at least one condition is True?"
            option4 = "A. or"
            option5 = "B. and"
            option6 = "C. not"
            correct2 = "A"

            question3 = "What does the not operator do?"
            option7 = "A. Adds two values"
            option8 = "B. Repeats a condition"
            option9 = "C. Reverses a condition"
            correct3 = "C"

        # CHAPTER 7
        elif chapter == "7":
            print("""
         ================= CHAPTER 7 =================
         INTRODUCTION TO ITERATION AND LOOPS

         Iteration means repeating a set of instructions
         until a certain condition is met or the sequence ends.

         FOR LOOP:
         Used to repeat code for each item in a sequence.

         Example:
         for number in range(1, 4):
             print(number)

         WHILE LOOP:
         Repeats code while a condition is True.

         Example:
         number = 1

         while number <= 3:
             print(number)
             number = number + 1

         RANGE FUNCTION:
         The range() function generates a sequence of numbers.

         BREAK STATEMENT:
         The break statement stops a loop.
         """)

            question1 = "Which loop is used to repeat code for each item?"
            option1 = "A. if"
            option2 = "B. for"
            option3 = "C. print"
            correct1 = "B"

            question2 = "Which loop repeats while a condition is True?"
            option4 = "A. while"
            option5 = "B. if"
            option6 = "C. elif"
            correct2 = "A"

            question3 = "Which keyword stops a loop?"
            option7 = "A. input"
            option8 = "B. range"
            option9 = "C. break"
            correct3 = "C"

        # QUIZ SECTION
        print("\n==============================================")
        quiz_choice = input("Do you want to take a quiz/activity? (Y/N): ").upper()

        if quiz_choice == "Y":
            print("\n=========== CHAPTER QUIZ =============")
            print("Answer each question by choosing A, B, or C.")

            correct = 0

            print("\n1.", question1)
            print(option1)
            print(option2)
            print(option3)
            answer1 = input("Your answer: ").upper()

            if answer1 == correct1:
                correct = correct + 1

            print("\n2.", question2)
            print(option4)
            print(option5)
            print(option6)
            answer2 = input("Your answer: ").upper()

            if answer2 == correct2:
                correct = correct + 1

            print("\n3.", question3)
            print(option7)
            print(option8)
            print(option9)
            answer3 = input("Your answer: ").upper()

            if answer3 == correct3:
                correct = correct + 1

            print("\n=============================")
            print("          QUIZ RESULT")
            print("===============================")

            if correct == 3:
                print("EXCELLENT! You got all the answers correct!")
            elif correct == 2:
                print("VERY GOOD! You understood most of the lesson.")
            elif correct == 1:
                print("GOOD! Keep practicing and reviewing.")
            else:
                print("NEEDS IMPROVEMENT. Review the lesson and try again.")

        elif quiz_choice == "N":
            print("\nOkay, thank you for using this chapter as your reviewer!")

        else:
            print("\nInvalid answer. Quiz skipped.")

        print("\n==============================================")
        next_lesson = input("Do you want to proceed to another lesson? (Y/N): ").upper()

        if next_lesson == "Y":
            print("\nReturning to the lesson choices...")

        elif next_lesson == "N":
            print("\nThank you for using Python Tutorial!")
            break

        else:
            print("\nInvalid answer. Returning to the lesson choices...")
