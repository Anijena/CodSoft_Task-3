# CodSoft_Task-3
import string
import random
len=int(input("Enter the length pf password:"))
print('''Choose set of character for your password
         1.Letters
         2.Digits
         3.Special char
         4.exit''')
ch=""
while True:
    choice=int(input("Enter a number from above:"))
    if(choice==1):
        ch=ch+string.ascii_letters
    elif(choice==2):
        ch=ch+string.digits
    elif(choice==3):
        ch=ch+string.punctuation
    elif(choice==4):
        break
    else:
        print("Please pick valid option")
password=[]
for i in range(len):
    r=random.choice(ch)
    password.append(r)
print("Random password is "+"".join(password))
        
        
