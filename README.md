# How-to-make-Formula-based-program

class math:
    def addition(x,y):
        print(x+y)
    def subs(x,y):
        print(x-y)
    def multi(x,y):
        print(x*y)
    def div(x,y):
        print(x/y)
        
class physics:
    def speed(distance,time):
        print("Speed = ",distance/time)
    def distance(speed,time):
        print("distance = ",speed*time)
    def time(distance,speed):
        print("time = ",distance/speed)
    
print("1. maths") 
print("2. science")

for i in range(3):
    userInput=int(input("= "))
    match userInput:
        case 1:
            print("1.addition")
            print("2.substraction")
            print("3.multiplication")
            print("4.division")
            user_input2=int(input("="))
            match user_input2:
                case 1:      
                    num1=int(input("First Number = "))     
                    num2=int(input("Second Number = "))    
                    math.addition(num1,num2)
                case 2:
                    num1=int(input("First Number = "))       
                    num2=int(input("Second Number = "))    
                    math.subs(num1,num2)
                case 3:
                    num1=int(input("First Number = "))       
                    num2=int(input("Second Number = "))    
                    math.multi(num1,num2)
                case 4:
                    num1=int(input("First Number = "))      
                    num2=int(input("Second Number = "))   
                    math.div(num1,num2)
    
    
    
    
        case 2:
            print("what you want to get !! ")
            print("1.distance")
            print("2.time ")
            print("3.speed ")
            user_input=int(input("="))
            match user_input:
                case 1: 
                    
                    speed=int(input("speed= "))
                    time =int (input("time = "))
                    physics.distance(speed,time)
                case 2:
                    distance=int(input("distance= "))
                    time =int (input("time = "))
                    physics.speed(distance,time)
                
                case 3:
                    distance=int(input("distance= "))
                    speed =int (input("speed = "))
                    physics.time(distance,speed)
                
                case _:
                    print("Hmm..! I think you  dont want to get anything ! ")
            
        case _:                            print("please input the mention above ! ")

