# my-own-bank
class Account:
    
    def init__(self,name,balance,min_balance):
      self.name=name
      self.balance=balance
      self.min_balance = min_balance

    def deposit(self,amount):
      self.balance += amount

    def withdraw(self,amount):
        
        if self.balance - amount>=self.min_balance:
            self.balance -=amount
        else:
           print("sorry not enough funds!")
            
    def statement(self):
      print("Account Balance: ${}".format(self.balance))

class Current(Account):
    def int__(self,name,balance):
      super().__init__(name,balance,min_balance =-1000)


        

        



