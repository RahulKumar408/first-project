
import random
def whowin(a, b):
# case when both you and computer chose same 
    if A == B:
        return None
# chek all possibility when computer chose snake 
    elif A == 's':
        if B == 'g':
            return True
        else:
            return False
# chek all possibility when computer chose water 
    elif A == 'w':
        if B == 's':
            return True
        else:
            return False
# chek all possibility when computer chose gun
    elif A == 'g':
        if B == 'w':
            return True
        else:
            return False

print("Computer chance:snake(s) or water(w) or gun(g)") 
rad_num = random.randint(1, 3) 
if rad_num == 1:
    A = 's'              
elif rad_num == 2:
    A = 'w'
elif rad_num == 3:
    A = 'g'

B = input("your chance:click s for snake w for water g for gun")
Call = whowin(A, B) 
print(f"computer chose {A}") 
print(f"you chose {B}") 
if Call == None:
    print("game draw") 
elif Call:
    print("you won") 
else:
    print("you lost") 






 
