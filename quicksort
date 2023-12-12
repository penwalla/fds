def partition(arr,left,right):
    i=left
    j=right
    pivot=arr[right]
    while i<j:
        while i<right and arr[i]<pivot:
            i+=1
        while j>left and arr[j]>pivot:
            j-=1
        if i<j:
            arr[i],arr[j]=arr[j],arr[i]

    arr[i],pivot=pivot,arr[i]
    return i

def quicksort(arr,left,right):
    if left<right:
        pos=partition(arr,left,right)
        quicksort(arr,pos+1,right)
        quicksort(arr,left,pos-1)
    
arr=[]
n = int(input("enter the number of element in the array : "))
for i in range(n):
    a = int(input("Enter the array elements : "))
    arr.append(a)
print("the array is is : ",arr)


quicksort(arr,0,len(arr)-1)
print("the sorted arry is : ",arr)
