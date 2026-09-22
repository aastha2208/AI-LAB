import random

class VacuumCleaner:
    def __init__(self):
        self.rooms = {
            "A": random.choice(["Dirty", "Clean"]),
            "B": random.choice(["Dirty", "Clean"])
        }
        self.current_room = random.choice(["A", "B"])

    def display(self):
        print("Current Room:", self.current_room)
        print("Room A:", self.rooms["A"])
        print("Room B:", self.rooms["B"])

    def clean(self):
        if self.rooms[self.current_room] == "Dirty":
            print("Room", self.current_room, "is dirty")
            print("Vacuum cleaner is sucking...")
            self.rooms[self.current_room] = "Clean"
        else:
            print("Room", self.current_room, "is already clean")

    def move(self):
        if self.current_room == "A":
            self.current_room = "B"
        else:
            self.current_room = "A"

        print("Moving to Room", self.current_room)

    def run(self):
        self.display()

        self.clean()
        self.move()
        self.clean()

        print("\nFinal State:")
        self.display()


v = VacuumCleaner()
v.run()
