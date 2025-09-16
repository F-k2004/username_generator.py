# username_generator.py
import rando

adjectives = ["Cool", "Happy", "Fast", "Smart", "Brave", "Epic", "Lazy", "Lucky"]
nouns = ["Tiger", "Ninja", "Coder", "Gamer", "Wizard", "Samurai", "Dragon", "Hero"]

def generate_username():
    adj = random.choice(adjectives)
    noun = random.choice(nouns)
    number = random.randint(10, 99)
    return f"{adj}{noun}{number}"

def main():
    print("🎭 تولیدکننده نام کاربری 🎭\n")
    while True:
        username = generate_username()
        print(f"نام کاربری پیشنهادی: {username}")
        again = input("می‌خوای یک نام دیگه بسازم؟ (y/n): ")
        if again.lower() != "y":
            print("👋 موفق باشی!")
            break

if __name__ == "__main__":
    main()
