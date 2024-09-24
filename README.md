# Compiler



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
