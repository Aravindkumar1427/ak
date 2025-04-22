dmk=0
admk=0
tvk=0
i=True
total=0
winner=""

while i==True:
    print(f'                           vote for your candidates....!'
          '\n                                  1.dmk'
          '\n                                  2.admk'
          '\n                                  3.tvk')
    
    vote=int(input("press number for vote="))
    if vote==1:
             dmk+=1
             total+=1
    elif vote==2:
        admk+=1
        total+=1
    elif vote==3:
        tvk+=1
        total+=1
    elif vote==000:
        if dmk>admk and dmk>tvk:
            winner=f"                   dmk is the winner total vote={dmk}.....!"
        elif admk>dmk and admk>tvk:
            winner=f"                   admk is the winner total vote={admk}.....!"
        elif tvk>dmk and tvk>admk:
            winner=f"                   tvk is the winner total votes={tvk}....!"   
        i=False
        
    
print(f"dmk ={dmk}\nadmk ={admk}\ntvk ={tvk}")
print(f"total_votes ={total}")
print(winner.upper())

