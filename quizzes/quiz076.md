# Quiz076

<img width="715" alt="Screen Shot 2023-09-13 at 11 36 05 AM" src="https://github.com/Lison18/Year-2/assets/116609563/1883a73c-4a7c-40c7-a4e9-489c5aa8f555">

# Code
```.py
class ErrorCheck:
    def __init__(self, data) -> None:
        self.data = data
        self.error = False
        self.output = 0

        length = len(self.data)
        first = self.data[0: length // 3]
        second = self.data[length // 3: (length // 3) * 2]
        third = self.data[(length // 3) * 2: length]

        for i in range(0, len(first)):
            if not first[i] == second[i] or not second[i] == third[i]:
                self.error = True
                self.output = int((int(first[i]) + int(second[i]) + int(third[i])) / 3)

test1 = ErrorCheck('100111001011001110010110011100101')
print(test1.error)
print(test1.output)

test2 = ErrorCheck('011101111101110111110111001111')
print(test2.error)
print(test2.output)
```
## Proof of work
<img width="1288" alt="Screen Shot 2023-09-13 at 11 40 27 AM" src="https://github.com/Lison18/Year-2/assets/116609563/6949e23f-42d9-4f77-8321-19d414a065ea">

