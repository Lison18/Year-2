# Quiz075

<img width="713" alt="Screen Shot 2023-09-13 at 11 27 35 AM" src="https://github.com/Lison18/Year-2/assets/116609563/b59a21d0-ca7e-4d0d-85a9-0967bcaa5a84">

# Code
```.py
class Binary:
    def __init__(self, inp) -> None:
        self.inp = inp
        self.output = self.words()

    def binary(self, char):
        return format(ord(char), '08b')

    def words(self):
        return ' '.join(map(self.binary, self.inp))

test1 = Binary('Hello World!')
print(test1.output)

test2 = Binary('42 is the answer.')
print(test2.output)

test3 = Binary('ABC123')
print(test3.output)
```

## Proof of work
<img width="1289" alt="Screen Shot 2023-09-13 at 11 28 53 AM" src="https://github.com/Lison18/Year-2/assets/116609563/18c55e6e-fec7-42cb-8704-e4e403789c62">


