# pair-of-number-using-python
l = [9,3,5,4,6,7,8,1,0]
l.sort()
print (l)
target = int(input("enter the number"))
left = 0
right = len(l) - 1
while (left <= right ):
    if (l[left] + l[right] > target):
        right = right -1
    elif (l[left] + l[right] < target):
        left = left + 1
    elif (l[left] + l[right] == target):
        print (l[left] , l[right])
        right = right -1
        left = left + 1

        

