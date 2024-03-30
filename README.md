# future
class Child:
    def __init__(self, name, age, gender):
        self.name = name
        self.age = age
        self.gender = gender
        self.is_sleeping = False

    def play(self, toy):
        return f"{self.name} is playing with {toy}."

    def sleep(self):
        self.is_sleeping = True
        return f"{self.name} is now sleeping."

    def wake_up(self):
        self.is_sleeping = False
        return f"{self.name} woke up!"

def main():
    # Creating instances of children
    child1 = Child("Alice", 5, "female")
    child2 = Child("Bob", 6, "male")

    # Performing actions
    print(child1.play("blocks"))
    print(child2.sleep())
    print(child1.wake_up())

if __name__ == "__main__":
    main()
