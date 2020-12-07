# Vehice-Management

#Here I am going to manage the counting and analyzing of vehicle in an organization

#li=[cycle,bus,rikshaw,count,amount]

li=[0,0,0,0,0]

def bus():

    li[1]=li[1]+1  #incrementing the nuber of buses
    
    li[3]=li[3]+1   #incremeinting the total number of vehicales
    

    li[4]=li[4]+100    #incrementing the amount
    
    print("Data enterd into the queue successfully")
    

def cycle():

    li[0]=li[0]+1   #incremanting the number of cycles
    
    li[3] = li[3] + 1  # incremeinting the total number of vehicales

    li[4] = li[4] + 20  # incrementing the amount
    
    print("Data enterd into the queue successfully")

def rikshaw():

    li[2]=li[2]+1 #incrementing the number of rikshaws
    
    li[3] = li[3] + 1  # incremeinting the total number of vehicales

    li[4] = li[4] + 50  # incrementing the amount
    
    print("Data enterd into the queue successfully")

def menue():

    ch=int(input("1.Enter for Bus\n2.Enter for Rikshaw\n3.Enter for Cycle\n4.Enter to print\n5.Enter for Delete\n6.Exit"))
    
    return ch

def delete():

    li[0]=0
    
    li[1] = 0
    
    li[2] = 0
    
    li[3]=0
    
    li[4] = 0
    
def details():

    print("Total number of bus:",li[1])
    
    print("Total number of Rikshaw:",li[2])
    
    print("Total number of cycle:",li[0])
    
    print("Total amount:",li[4])
    
    print("Total number of vehicals:",li[3])
    

if __name__ == '__main__':

 while 1:
 
    print("This is a small management of data to the vehicales:")
    
    a=menue()
    
    if a ==1:
    
        bus()
        
    elif a==2:
    
        rikshaw()
        
    elif a==3:
    
        cycle()
        
    elif a==4:
    
        details()
        
    elif a==5:
    
        delete()
        
    elif a==6:
    
        exit()




