# Compiler
TIME----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


import time
t1=time.time()
print("t1=",t1)
for i in range(100):
  print(i,end="")
print()
t2=time.time()
print("t2=",t2)
print("execution time before loop unrolling :", t2-t1)
for i in range (100):
  print(i,end=" ")
  print(i+1,end=" ")
  print(i+2,end=" ")
  print(i+3,end=" ")
  print(i+4,end=" ")
print()
t3=time.time()
print("t3=",t3)
print("execution time after loop unrolling ",t3-t2)
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
inputstring

def FA(s):
    if len(s)<3:
        return "REJECTED"
    if s[:3]=="101":
        for i in range (3,len(s)):
            if s[i]==0:
                return "Rejected"
        return "accepted"
    return "rejected"
input_string=['1','10101','101','10111','01010','100','1011101']
for i in input_string:
    print(f"input: {i} -> {FA(i)}")
