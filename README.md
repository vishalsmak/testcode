check=1
while(check):
    x=list(input('enter the string :'))
    data=[]
    data=data+x
    length=len(data)-1
    i=0
    flage=0
    flago=0
    
    if((length/2)%2==0):
        for z in range(length/2-1):
            if (data[i]==data[(length-1)-i]):
                flage+=1
                if (flage==length/2):
                    print "is a palidrome"
            else:
                print "not a palindrome"
                break
    if((length/2)%2!=0):
        for z in range(((length-1)/2)-1):
            if (data[z]==data[(length-1)-z]):
                flago+=1
                if (flago==(length-1)/2):
                    print "is a palidrome"
            elif(data[z]!=data[(length-1)-z]):
                print "not a palindrome"
                break
    check=0
    check=int(input("do you want to start again 1/0"))


                
          
