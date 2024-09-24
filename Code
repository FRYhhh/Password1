import re

def check_password_strength(password):
    errors = []

    if len(password) < 8:
        errors.append("Пароль слишком короткий. Длина должна быть не менее 8 символов.")

    if not re.search(r'[A-Z]', password):
        errors.append("Пароль должен содержать хотя бы одну заглавную букву.")

    if not re.search(r'[a-z]', password):
        errors.append("Пароль должен содержать хотя бы одну строчную букву.")

    if not re.search(r'[0-9]', password):
        errors.append("Пароль должен содержать хотя бы одну цифру.")

    if not re.search(r'[!@#$%&]', password):
        errors.append("Пароль должен содержать хотя бы один специальный символ (!, @, #, $, %, &).")

    if errors:
        return "Найдены следующие проблемы с паролем:\n" + "\n".join(errors)
    else:
        return "Пароль действительный!"

if name == "main":
    password = input("Введите пароль для проверки: ")
    result = check_password_strength(password)
    print(result)
