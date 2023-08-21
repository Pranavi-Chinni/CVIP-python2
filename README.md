import time
def calculate_typing_speed(input_text, elapsed_time):
    words = input_text.split()
    word_count = len(words)
    time_in_minutes = elapsed_time / 60
    wpm = word_count / time_in_minutes
    return wpm
def main():
    prompt_text = "The quick brown fox jumps over the lazy dog."
    print("Type the following sentence:")
    print(prompt_text)
    input("Press Enter when you are ready to start...")
    start_time = time.time()
    typed_text = input("Type the sentence: ")
    end_time = time.time()
    elapsed_time = end_time - start_time
    typing_speed = calculate_typing_speed(typed_text, elapsed_time)
    print("\nTime taken: {:.2f} seconds".format(elapsed_time))
    print("Your typing speed: {:.2f} WPM".format(typing_speed))
if __name__ == "__main__":
    main()



Output:

C:\Users\chinn\PycharmProjects\pythonProject\venv\Scripts\python.exe C:\Users\chinn\PycharmProjects\pythonProject\main.py 
Type the following sentence:
The quick brown fox jumps over the lazy dog.
Press Enter when you are ready to start...
Type the sentence: The quick brown fox jumps over the lazy dog.

Time taken: 22.02 seconds
Your typing speed: 24.53 WPM

Process finished with exit code 0
