# Базовий клас Тварина
class Tvarina:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def info(self):
        return f"{self.name}, {self.age} років."

# Підклас Собака
class Sobaka(Tvarina):
    def speak(self):
        return "Гав!"

# Підклас Кіт
class Kit(Tvarina):
    def speak(self):
        return "Мяу!"

# Приклади використання
sobaka = Sobaka("Барсик", 3)
kit = Kit("Мурчик", 2)

print(sobaka.info(), sobaka.speak())  # Барсик, 3 років. Гав!
print(kit.info(), kit.speak())        # Мурчик, 2 років. Мяу!
