# carclass Car:
    def __init__(self, make, model, year, color):
        self.make = make
        self.model = model
        self.year = year
        self.color = color
        self.speed = 0

    def accelerate(self, increment):
        self.speed += increment
        print(f"The car is now moving at {self.speed} km/h.")

    def brake(self, decrement):
        if self.speed >= decrement:
            self.speed -= decrement
            print(f"The car slowed down to {self.speed} km/h.")
        else:
            self.speed = 0
            print("The car stopped.")

    def display_info(self):
        print("Car Information:")
        print(f"Make: {self.make}")
        print(f"Model: {self.model}")
        print(f"Year: {self.year}")
        print(f"Color: {self.color}")
