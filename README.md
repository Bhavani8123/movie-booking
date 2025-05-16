# movie-booking
user=[]
password=[]
s_seats1=['s1','s2','s3','s4']
s_seats2=['s1','s2','s3','s4']
s_seats3=['s1','s2','s3','s4']
b_seats1=['s1','s2','s3','s4']
b_seats2=['s1','s2','s3','s4']
b_seats3=['s1','s2','s3','s4']
j_seats1=['s1','s2','s3','s4']
j_seats2=['s1','s2','s3','s4']
j_seats3=['s1','s2','s3','s4']
class movie():
    def login(self,list1,list2,):
        print("login page")
        self.list1=list1
        self.list2=list2 
        u1=input("enter your name:")
        list1.append(u1)
        while(1):
            passw=input("enter your password : ")
            lower_case=['a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z']
            upper_case=['A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z']
            numeric=['1','2','3','4','5','6','7','8','9','0']
            special=['!','@','#','$','%','^','&','*']
            lc=uc=num=sp=0
            for i in range(len(passw)):
                if passw[i] in lower_case:
                    lc+=1
                elif passw[i] in upper_case:
                    uc+=1
                elif passw[i] in numeric:
                    num+=1
                elif passw[i] in special:
                    sp+=1
            if(lc>=1 and uc>=1 and num>=1 and sp>=1):
                list2.append(passw)
                break
            elif(lc==0 or uc==0 or num==0 or sp==0):
                print("atleast one upper and lower case letters and numbers and special characters in your password")
                print("try again")
        print("login successfully")
    def seat1(self,s_seats1,s_seats2,s_seats3):
        print("movies are:")
        print("1.kalki 2.tholiprema 3.kushi")
        a1=int(input("movie option "))
        if(a1==1):
            print("available seats are: ")
            print(*s_seats1)
            print("select your seat:")
            s=input()
            if(s in s_seats1):
                print("200rs for seat")
                bank=input("enter your account number: ")
                while(1):
                    aa=input("enter YES for draw the money 200: ")
                    if(aa=='YES'):
                        print("payment successfully")
                        print("your seat is booked")
                        s_seats1.remove(s)
                        break
                    else:
                        print("invalid input")
            else:
                print("already booked")
        elif(a1==2):
            print("available seats are: ")
            print(*s_seats2)
            print("select your seat:")
            s=input()
            if(s in s_seats2):
                print("200rs for seat")
                bank=input("enter your account number: ")
                while(1):
                    aa=input("enter YES for draw the money 200: ")
                    if(aa=='YES'):
                        print("payment successfully")
                        print("your seat is booked")
                        s_seats2.remove(s)
                        break
                    else:
                        print("invalid input")
            else:
                print("already booked")
        else:
            print("available seats are: ")
            print(*s_seats3)
            print("select your seat:")
            s=input()
            if(s in s_seats3):
                print("200rs for seat")
                bank=input("enter your account number: ")
                while(1):
                    aa=input("enter YES for draw the money 200: ")
                    if(aa=='YES'):
                        print("payment successfully")
                        print("your seat is booked")
                        s_seats3.remove(s)
                        break
                    else:
                        print("invalid input")
            else:
                print("already booked")
    def seat2(self,j_seats1,j_seats2,j_seats3):
        print("movies are:")
        print("1.kalki 2.tholiprema 3.kushi")
        a1=int(input("movie option "))
        if(a1==1):
            print("available seats are: ")
            print(*j_seats1)
            print("select your seat:")
            s=input()
            if(s in j_seats1):
                print("100rs for seat")
                bank=input("enter your account number: ")
                while(1):
                    aa=input("enter YES for draw the money 100: ")
                    if(aa=='YES'):
                        print("payment successfully")
                        print("your seat is booked")
                        j_seats1.remove(s)
                        break
                    else:
                        print("invalid input")
            else:
                print("already booked")
        elif(a1==2):
            print("available seats are: ")
            print(j_seats2)
            print("select your seat:")
            s=input()
            if(s in j_seats2):
                print("100rs for seat")
                bank=input("enter your account number: ")
                while(1):
                    aa=input("enter YES for draw the money 100: ")
                    if(aa=='YES'):
                        print("payment successfully")
                        print("your seat is booked")
                        j_seats2.remove(s)
                        break
                    else:
                        print("invalid input")
            else:
                print("already booked")
        else:
            print("available seats are: ")
            print(*j_seats3)
            print("select your seat:")
            s=input()
            if(s in j_seats3):
                print("100rs for seat")
                bank=input("enter your account number: ")
                while(1):
                    aa=input("enter YES for draw the money 100: ")
                    if(aa=='YES'):
                        print("payment successfully")
                        print("your seat is booked")
                        j_seats3.remove(s)
                        break
                    else:
                        print("invalid input")
            else:
                print("already booked")
        
    def seat3(self,b_seats1,b_seats2,b_seats3):
        print("movies are:")
        print("1.kalki 2.tholiprema 3.kushi")
        a1=int(input("movie option: "))
        if(a1==1):
            print("available seats are: ")
            print(*b_seats1)
            print("select your seat:")
            s=input()
            if(s in b_seats1):
                print("150rs for seat")
                bank=input("enter your account number: ")
                while(1):
                    aa=input("enter YES for draw the money 150: ")
                    if(aa=='YES'):
                        print("payment successfully")
                        print("your seat is booked")
                        b_seats1.remove(s)
                        break
                    else:
                        print("invalid input")
            else:
                print("already booked")
        elif(a1==2):
            print("available seats are: ")
            print(*b_seats2)
            print("select your seat:")
            s=input()
            if(s in b_seats2):
                print("150rs for seat")
                bank=input("enter your account number: ")
                while(1):
                    aa=input("enter YES for draw the money 150: ")
                    if(aa=='YES'):
                        print("payment successfully")
                        print("your seat is booked")
                        b_seats2.remove(s)
                        break
                    else:
                        print("invalid input")
            else:
                print("already booked")
        else:
            print("available seats are: ")
            print(*b_seats3)
            print("select your seat:")
            s=input()
            if(s in b_seats3):
                print("150rs for seat")
                bank=input("enter your account number: ")
                while(1):
                    aa=input("enter YES for draw the money 150: ")
                    if(aa=='YES'):
                        print("payment successfully")
                        print("your seat is booked")
                        b_seats3.remove(s)
                        break
                    else:
                        print("invalid input")
            else:
                print("already booked")
    def movies(self,s_seats1,s_seats2,s_seats3,b_seats1,b_seats2,b_seats3,j_seats1,j_seats2,j_seats3):
        print("theators are: 1.sri theator 2.bhanu theator 3.janu theator")
        p=int(input("if you want go back please enter 1, otherwise enter any number: "))
        if(p!=1):
            option=int(input("enter your option for above theators"))
            if(option==1):
                self.seat1(s_seats1,s_seats2,s_seats3)
            elif(option==2):
                self.seat2(j_seats1,j_seats2,j_seats3)
            elif(option==3):
                self.seat3(b_seats1,b_seats2,b_seats3)
        else:
            pass
    def logout(self):
        print("logout successfully")

o=movie()
while(1):
    u=int(input("if you want login enter 1 othrwise enter any number: "))
    if(u==1):
        o.login(user,password)
        while(1):
            #o.login(user,password)
            print("available theators ")
            o.movies(s_seats1,s_seats2,s_seats3,j_seats1,j_seats2,j_seats3,b_seats1,b_seats2,b_seats3)
            oo=int(input("if you want logout please enter 1 other wise enter anny number:"))
            if(oo==1):
                o.logout()
                break
    else:
        break
        

    


    
