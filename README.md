# Assignment-5-OOPs



Challenge 2: Implement a Calculator Class

class calculator:
    def __init__(self):
        self.num1 = eval(input('Enter the value 1 :'))
        self.num2 = eval(input('Enter the value 2 :'))   
    def sum(self):
        print(self.num1 + self.num2)
    def min(self):
        print(self.num1 - self.num2)
    def multi(self):
        print(self.num1 * self.num2)
    def div(self):
        print(self.num1 / self.num2)
                               
opr= input('Enter the opr..')
obj = calculator()

if opr == '+':
    obj.sum()
elif opr == '-':
    obj.min()
elif opr == '*':
    obj.multi()
elif opr == '/':
    obj.div()
else:
    print('invalid operation')                               

