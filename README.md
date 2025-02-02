# as143
yes or no
import random

def get_random_answer():
    answers = ["نعم", "لا"]
    return random.choice(answers)

# محاكاة ضغط الزر
def press_button():
    input("اضغط زر الإدخال (Enter) للحصول على إجابة...")
    answer = get_random_answer()
    print(f"الإجابة هي: {answer}")

# تشغيل اللعبة
while True:
    press_button()
    play_again = input("هل تريد المحاولة مرة أخرى؟ (اكتب 'نعم' أو 'لا'): ").strip().lower()
    if play_again != 'نعم':
        print("شكرًا للعب! 😊")
        break
