# maximum-of-all-sub-array
#actully mamaji this program is given( unsupported operand type(s) for +: 'int' and 'str') this error on line no 9 so many times i try and #i also search on google but i dont understand plz help me 
#ques.--Given an array and an integer k, find the maximum for each and every contiguous subarray of size k.

test_case=int(input())
for i in range(test_case):
    line=input().split()
    n=line[0]
    k=line[1]
    arr=[int(n) for n in input().split()]
    maxima = list()
    p = 0
    while p+k-1 <= n-1:
        maxima.append(max(arr[p:p+k]))
        p+=1
    for m in maxima:
        print(m,end=" ")
    print("")



