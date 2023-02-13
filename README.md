class Animal:
    def __init__(self, name, species):
        self.name = name
        self.species = species

    def __str__(self):
        return f"{self.name} is a {self.species}"

class Dog(Animal):
    def __init__(self, name, breed):
        Animal.__init__(self, name, species="Dog")
        self.breed = breed

    def __str__(self):
        return f"{self.name} is a {self.breed} {self.species}"

dog = Dog("Buddy", "Labrador")
print(dog)

