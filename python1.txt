class MyException(Exception):

    def __init__(self,v):
        self.v=v
    def __str__(self):
        return str (self.v)



def xyz(a,b):

    sum = a + b

    if sum < 150:
        raise MyException('Custom Exception Occurred')
    else:
        return sum

a = int(input())
b = int(input())
print(xyz(a,b))
