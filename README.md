'''write a program to read a character untill * is entered. count the number of upper case,lower case, and numbers entered by the users '''
ch=input("enter the character:")
n=u=l=0
if ch>='0' and ch<='9':
    n+=1
elif ch>='a' and ch<='z':
    l+=1
elif ch>='A' and ch<='Z':
    u+=1
while ch!='*':
    ch=input("enter the any character:")
    if ch>='0' and ch<='9':
        n+=1
    elif ch>='a' and ch<='z':
        l+=1
    elif ch>='A' and ch<='Z':
        u+=1
    print("lowercase char:",l)
    print("uppercase char:",u)
    print("the number are:",n)
OUTPUT:
enter the character: e
enter the any character: 3
lowercase char: 1
uppercase char: 0
the number are: 1
enter the any character: A
lowercase char: 1
uppercase char: 1
the number are: 1
enter the any character: U
lowercase char: 1
uppercase char: 2
the number are: 1
enter the any character: 3
lowercase char: 1
uppercase char: 2
the number are: 2
enter the any character: e
lowercase char: 2
uppercase char: 2
the number are: 2
#simple for loop with string
str='cheetah'
for i in str:
    print(i,end=' ')
OUTPUT:
c h e e t a h
#for with-in range
n=int(input("enter the value of n"))
for i in range(1,n+1):
    print(i,end=' ')
for i in range(n,0,-1):
    print(i,end=' ')
OUTPUT:
enter the value of n 10
1 2 3 4 5 6 7 8 9 10 10 9 8 7 6 5 4 3 2 1 
#code for printing multiplication table n,where n is entered by the user 
'''input:
enter any number:2
output:
multiplication table of 2'''
n=int(input("enter the number"))
for i in range(0,11):
    print(n,"x",i,"=",n*i)
OUTPUT:
enter the number 17
17 x 0 = 0
17 x 1 = 17
17 x 2 = 34
17 x 3 = 51
17 x 4 = 68
17 x 5 = 85
17 x 6 = 102
17 x 7 = 119
17 x 8 = 136
17 x 9 = 153
17 x 10 = 170
n=int(input("enter the year"))
ed=int(input("enter the year"))
for i in range(n,ed+1):
    if i%4==0:
        print(i,end=' ')
output:
enter the year 1900
enter the year 2101
1900 1904 1908 1912 1916 1920 1924 1928 1932 1936 1940 1944 1948 1952 1956 1960 1964 1968 1972 1976 1980 1984 1988 1992 1996 2000 2004 2008 2012 2016 2020 2024 2028 2032 2036 2040 2044 2048 2052 2056 2060 2064 2068 2072 2076 2080 2084 2088 2092 2096 2100 
n=int(input("enter the value of n"))
s=0
for i in range(1,n+1):
    a=1/(i**2)
    s+=a
print(s)
output:
enter the value of n 5
1.4636111111111112
n=int(input("enter the value of n"))
s=0
for i in range(1,n+1):
    a=(i**i)/i
    s+=a
print(s)
output:
enter the value of n 5
701.0
'''generating a calender manually'''
sday=int(input("enter the start day of th month(1-7):"))
numday=int(input("enter the number of days"))
print("Sun  Mon  Tue  Wed  Thu  Fri  Sat")
print("---------------------------------")
for i in range(sday-1):
    print(end="    ")
i=sday-1
for j in range(1,numday+1):
    if i>6:
        print( )
        i=1
    else:
        i+=1
    print(str(j)+ "  ",end=' ')
OUTPUT:
enter the start day of th month(1-7): 1
enter the number of days 31
Sun  Mon  Tue  Wed  Thu  Fri  Sat
---------------------------------
1    2    3    4    5    6    7   
8    9    10   11   12   13   14   
15   16   17   18   19   20   21   
22   23   24   25   26   27   28   
29   30   31   
''generating a calender manually''
mdays=31
sday=2
print("Sun  Mon  Tue  Wed  Thu  Fri  Sat")
for _ in range(sday):
    print("   ",end=' ')
for days in range(1,mdays+1):
    print(f"{days:>3}",end=' ')
    if(sday+days)%7==0:
        print()
OUTPUT:
Sun  Mon Tue Wed Thu Fri Sat
          1   2   3   4   5 
  6   7   8   9  10  11  12 
 13  14  15  16  17  18  19 
 20  21  22  23  24  25  26 
 27  28  29  30  31 
