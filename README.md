arr=[9.00,9.40,9.50,11.00,15.00,18.00]
dep=[9.10,12.00,11.20,11.30,19.00,20.00]
dep.sort()
n=len(arr)

for i in range(n):
    plat=1
    for j in range(n):
        if(arr[i]>=arr[j] and dep[j]>=arr[i]):
            plat+=1
print(plat)