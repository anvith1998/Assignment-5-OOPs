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


Challenge 4: Implement a Banking Account

class Bank_Account:
    def __init__(self):
        self.balance=0
        print("Hello!!! Welcome to the Deposit & Withdrawal Machine")
 
    def deposit(self):
        amount=float(input("Enter amount to be Deposited: "))
        self.balance += amount
        print("\n Amount Deposited:",amount)
 
    def withdraw(self):
        amount = float(input("Enter amount to be Withdrawn: "))
        if self.balance>=amount:
            self.balance-=amount
            print("\n You Withdrew:", amount)
        else:
            print("\n Insufficient balance  ")
 
    def display(self):
        print("\n Net Available Balance=",self.balance)
 
s = Bank_Account()
  
s.deposit()
s.withdraw()
s.display()
