# Quiz076
```.py
class parity_check:
    def __init__(self, data) -> None:
        self.data = data
        self.ones = 0
        self.output = False
        self.Error()

    def Error(self):
        for i in range(1, len(self.data)):
            if self.data[i] == '1':
                self.ones += 1

            if (self.data[0] == '1' and self.ones%2==0) or (self.data[0]=='0' and self.ones%2==1):
                self.output = False
            else:
                self.output = True

test1 = parity_check("100111001011001110010110011100101")
print(test1.output)

test2 = parity_check("011101111101110111110111001111")
print(test2.output)
```

## Proof of work

<img width="1224" alt="Screen Shot 2023-09-13 at 11 31 17 AM" src="https://github.com/Lison18/Year-2/assets/116609563/e72d79ee-4efd-4c31-bba2-75eff5430404">

