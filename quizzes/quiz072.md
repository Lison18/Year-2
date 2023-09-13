# Quiz 072

<img width="717" alt="Screen Shot 2023-09-13 at 11 19 06 AM" src="https://github.com/Lison18/Year-2/assets/116609563/bc8cc9b9-4091-4fc2-b47a-aa2507695f16">

# Code

```.py
import random

class MacAddressGenerator:
    def __init__(self, amount) -> None:
        self.chars = '0123456789ABCDEF'
        self.adr = ''
        self.amount = amount
        self.generate()

    def generate(self):
        for _ in range(self.amount):
            self.adr += self.char_generator() + self.char_generator() + ':'
        self.adr = self.adr[:-1]

    def char_generator(self):
        rand = random.randint(0, 15)
        return self.chars[rand]

class MacGenerator:
    def __init__(self, N):
        self.N = N
        self.output = []
        self.generate_mac_addresses()

    def generate_mac_addresses(self):
        for _ in range(self.N):
            mac = MacAddressGenerator(6)
            self.output.append(mac.adr)

test1 = MacGenerator(4)
print(test1.output)

class MacGeneratorWithMaker:
    def __init__(self, N, maker):
        self.N = N
        self.maker = maker
        self.output = []
        self.generate_mac_addresses()

    def generate_mac_addresses(self):
        for _ in range(self.N):
            mac = MacAddressGenerator(3)
            output = f"{self.maker}:{mac.adr}"
            self.output.append(output)

test2 = MacGeneratorWithMaker(5, "AA:AA:AA")
print(test2.output)
```

## Proof of work

<img width="1069" alt="Screen Shot 2023-09-13 at 11 20 23 AM" src="https://github.com/Lison18/Year-2/assets/116609563/f32379e8-da25-4f23-820c-29504e69f2d3">

