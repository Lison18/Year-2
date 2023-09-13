# Quiz 071

<img width="746" alt="Screen Shot 2023-09-13 at 11 16 59 AM" src="https://github.com/Lison18/Year-2/assets/116609563/be5b12e5-f2c1-4761-9ef1-41e1400f229b">

# Code
```.py
import random

class IPV6:
    def __init__(self):
        self.adr = ':'.join(''.join(random.choice('0123456789ABCDEF') for _ in range(4)) for _ in range(8))

class IPV6Machine:
    def __init__(self, N):
        self.N = N
        self.output = [IPV6().adr for _ in range(self.N)]

test1 = IPV6Machine(5)
print(test1.output)

test2 = IPV6Machine(3)
print(test2.output)
```

## Proof of work

<img width="1326" alt="Screen Shot 2023-09-13 at 11 18 03 AM" src="https://github.com/Lison18/Year-2/assets/116609563/cb822e18-d0ae-4da4-90a8-2fa6e798c48b">
