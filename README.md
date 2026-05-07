import sys

def generate_text(prompt):
    return f"AI response: {prompt}"

def main():
    # If no input system is available, use a default value
    if sys.stdin.isatty():
        user_input = input("Enter a prompt: ")
    else:
        user_input = "default prompt"

    result = generate_text(user_input)
    print(result)

if __name__ == "__main__":
    main()
