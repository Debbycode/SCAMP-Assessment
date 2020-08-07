# This is a SCAMP Technical Assessment to be submitted for She Code Africa Application

# Python Function for Fibbonacci Sequence

def Fibbonacci_sequence(Number):
    if (Number==0):                                                          # To check whether the given number is 0 or not. 
        return 0                                                             # if true, this function returns the value 0
    
    
   elif (Number==1):                                                       # To check whether the given number is 1 or not.
        return 1                                                            # if true, this function returns the value 1
    
    
   else:                                                                   # if given number is greater than 1, then the function in else block is executed
        return (Fibbonacci_sequence(Number-2)
               + Fibbonacci_sequence(Number-1))
               
    
Number =int(input("\nDear User, Enter a Value Please:  "))                   # function requests input number
print("\nFibbonacci_sequence: ", end = '  ')


for n in range (0, Number):
    print(Fibbonacci_sequence(n), end = '  ')                                 #displays result
