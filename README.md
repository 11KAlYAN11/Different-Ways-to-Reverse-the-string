# Different-Ways-to-Reverse-the-string

date 20/08/2022

different ways to reverse the string


"""def revstr(str):
    str1 = ''
    for i in str:
        str1 = i+str1# 1)k+'' 2) ak + '' 3) lak + '' 4) ylak + '' 5) aylak...
    return str1

name = input("Enter String to Reverse: ")
print(revstr(name))"""



"""name = input("Enter String to Reverse: ")
l = len(name) - 1
revstr = ""
while(l >= 0):
    revstr =  revstr + name[l]
    l-=1
print(revstr)"""


"""name = input("Enter String to Reverse: ")
s = "".join(reversed(name))
print(s)
"""

"""def reverse(str):   
    if len(str) == 0: # Checking the lenght of string  
        return str   
    else:   
        return reverse(str[1:]) + str[0]   
    
str = "Devansh Sharma"   
print ("The original string  is : ", str)     
print ("The reversed string(using recursion) is : ", reverse(str))  
"""


# Function to reverse a string
'''def reverse(string):
    string = [string[i] for i in range(len(string)-1, -1, -1)]
    return "".join(string)

s = "AsamKalyan"                                                          
print("The original string  is : ", s)
print("The reversed string(using reversed) is : ", reverse(s))
'''




#program to find at which index substring occurs and total counts
s = input("Enter a main string : ")
sub = input("Enter a sub string : ")
pos = -1 #main
while True:
    pos = s.find(sub,pos+1,len(s))
    if pos == -1:
        break
    print("found at ",pos)
print("no of occurances = ",s.count(sub))



