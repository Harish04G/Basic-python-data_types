# Basic-python-data_types
#Data types in python

 # 1.string
 
#Example 
 
Q1="How are you?"
Q2="I'm good"
print(type(Q2))
print(Q1[0:3])#slicing

print(Q1[11])#indexing

str_replace=Q2.replace('good','bad')#replacing
print(str_replace)

str_rev = Q2[::-1]#reversing
print(str_rev)

find_length=len(Q1)#finding length of the string
print(find_length)

#2.tuple

#Example 

month=("jan","feb","mar","apr","may")
print(type(month))

print(month)

print(month[0])#indexing
       
find_index=month.index("feb")#find position of the index
print(find_index)

con=month.count("mar")#counting the specific element
print(con)

month+=("jun",)#concatenation in tuple
print(month)

#nested tuple
company=(1,1001,["Harish","Production department"])#intermixing data types
print(company)

#2.List

#Example 

company=[1,1001,"Raj","sales department"]
print(type(company))

print(company)

print(company[0])#indexing
       
find_index=company.index("Raj")#find position of the index
print(find_index)

com=company.count("sales department")#counting the specific element
print(com)

company+=["Present",]#concatenation in list
print(company)

con=len(company)#couting the length of the list 
print(con)

a=[]#In list empty list also possible
print(type(a))

a=[48,11,23,50,94,80]
print(a)

a.extend([1])
print(a)

a.insert(3,5)#adding specific element in a list it stored in specific path as you mentioned
print(a)

a.append(10)#adding specific element in a list it defaultly stored last element in a list
print(a)

a.sort()# arranging in ascending order
print(a)

a.reverse()#arranging in desending order
print(a)

a.remove(11)#removing specific element
print(a)

a.pop()#it defaultly removing last element from the list
print(a)

a.clear()#it is used to clear the list totally
print(a)

#nested list
b=[101,203,("Hello Harish!"),{1:"wELCOME"}] #intermixing data types
print(b)


#Dictionary
#Example 
mydict={}#Empty dictionary
print(type(mydict))
#In dictionary we can change the value but we cannot the key,in dictionary key is always unique
names={1:"Harish",2:"Deepak",3:"Ram kumar",4:"Santhosh"}
print(names)
print(names[1])#dictionary is indexable by key not by memory index

#dict using for loop
for key,val in names.items():#getting both key and value
    print(key,val)

for items in names.keys():#getting only keys
    print(items)

for items in names.values():#getting only values
    print(items)


#Set
#Example
num={1,2,3,2}
print(type(set))

print(set)

num1={4,3,5,4,1,3}
result=num|num1
print(result)#It does not allow duplicate value

num.add(12)
print(num)
