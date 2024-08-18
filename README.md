# coffeeclass Coffee:
    def __init__(self, coffee_type="Black Coffee"):
        self.coffee_type = coffee_type
        self.sugar = 0
        self.milk = False

    def add_sugar(self, teaspoons):
        self.sugar += teaspoons
        print(f"Added {teaspoons} teaspoon(s) of sugar.")

    def add_milk(self):
        self.milk = True
        print("Added milk.")

    def serve(self):
        milk_status = "with milk" if self.milk else "without milk"
        sugar_status = f"with {self.sugar} teaspoon(s) of sugar" if self.sugar > 0 else "without sugar"
        print(f"Serving {self.coffee_type} {milk_status} and {sugar_status}. Enjoy your coffee!")


# Example usage:
my_coffee = Coffee("Latte")

my_coffee.add_sugar(2)
my_coffee.add_milk()
my_coffee.serve()
