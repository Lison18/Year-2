# quiz 017

<img width="658" alt="Screen Shot 2023-09-13 at 11 05 10 AM" src="https://github.com/Lison18/Year-2/assets/116609563/896e3a55-1ad3-47db-9b3e-8f2f6b5c6009">

# Code

**.Py import math
ips = []

def ipv4Machine():
    for i in range(1, 255**4+1):
        a = math.floor(i / 255 / 255 / 255 % 255)
        b = math.floor(i / 255 / 255 % 255)
        c = math.floor(i / 255 % 255)
        d = math.floor(i % 255)
        ips.append(f"{a}:{b}:{c}:{d}")

ipv4Machine()

print(ips)

def ipvyMachine2():
    for a in range(1,255):
        for b in range(1,255):
            for c in range(1,255):
                for d in range(1,255):
                    ips.append(f"{a}:{b}:{c}:{d}")
