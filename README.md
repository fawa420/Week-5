turn = 0
a=1
b=2
c=3
d=4
e=5
f=6
g=7
h=8
i=9
print(f"""
            |{a}| |{b}| |{c}|
            |{d}| |{e}| |{f}|
            |{g}| |{h}| |{i}|
      """)

while (True) :
   if (turn == 0):
    X=int(input("Player 1 : Enter a no. 0 to 9"))
    if ( X==1 ):
      a='x'
    elif ( X==2):
     b ='x'
    elif ( X==3):
     c ='x'
    elif ( X==4):
     d ='x'
    elif ( X==5):
     e ='x'
    elif ( X==6):
     f ='x'
    elif ( X==7):
     g ='x'
    elif ( X==8):
     h ='x'
    elif ( X==9):
     i ='x'
    else :
     print("enter a valid no.")
     turn-=1
    turn+=1
   if (turn ==1):
    Y=int(input(" Player 2 : Enter a no. 0 to 9"))
    if ( Y==1 ):
      a='y'
    elif ( Y==2):
     b ='y'
    elif ( Y==3):
     c ='y'
    elif ( Y==4):
     d ='y'
    elif ( Y==5):
     e ='y'
    elif ( Y==6):
     f ='y'
    elif ( Y==7):
     g ='y'
    elif ( Y==8):
     h ='y'
    elif ( Y==9):
     i ='y'
    else :
     print("enter a valid no.")
     turn==1
    turn-=1
   print(f"""
            |{a}| |{b}| |{c}|
            |{d}| |{e}| |{f}|
            |{g}| |{h}| |{i}|
      """)
   if ( a=='x' and b=='x'and c=='x' or (d=='x' and e=='x'and f=='x') or  ( g=='x' and h=='x'and i=='x') or (a=='x' and e=='x'and i=='x') or (c=='x' and e=='x'and g=='x') or(a=='x' and d=='x'and g=='x') or (b=='x' and e=='x'and h=='x') or (c=='x' and f=='x'and i=='x')):
    print("Player 1 win ")
    break
   elif ( a=='y' and b=='y'and c=='y' or (d=='y' and e=='y'and f=='y') or  ( g=='y' and h=='y'and i=='y') or (a=='y' and e=='y'and i=='y') or (c=='y' and e=='y'and g=='y') or(a=='y' and d=='y'and g=='y') or (b=='y' and e=='y'and h=='y') or (c=='y' and f=='y'and i=='y')):
    print("Player 2 win ")     
    break
