# constr-destr
# inserting a value in an index of a no.
class numbers:
    def __init__(self,mylist):
        self.mylist=mylist
    def __getitem__(self,index):
        return self.mylist[index]
    def __setitem__(self,index,value):
        self.mylist[index]=value
numlist=numbers([1,2,3,4,5,6,7,8,9])
print(numlist[7])
numlist[3]=30
print(numlist.mylist)

# output
8
[1, 2, 3, 30, 5, 6, 7, 8, 9]
