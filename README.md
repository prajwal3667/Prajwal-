# Prajwal-
#My first repository on Git Hub
''' Project is based for students management system in python for beginners 
print(""" 

  ------------------------------------------------------
 |======================================================| 
 |======== Welcome To Student Management System	========|
 |======================================================|
  ------------------------------------------------------
""")
Dict={}
while True:
    print("""
    Enter 1 : To Add New Student:
    Enter 2 : To Search Student:
    Enter 3 : To Remove Student:
    Enter 4 : Exit system		
		""")
    Choice=input('please select the given option:')
    if int(Choice)==1:
        Roll=int(input('Enter roll num:'))
        if Roll in Dict:
            print('\nRoll number already exist:')
            Dict[Roll]={}
            Dict[Roll]['name']=input('\nEnter student name:')
            Dict[Roll]['Science']=int(input('\nEnter Student Marks:'))
            Dict[Roll]['M2']=int(input('\nEnter Student Marks:'))
        else:
            Dict[Roll]={}
            Dict[Roll]['name']=input('\nEnter student name:')
            Dict[Roll]['Science']=int(input('\nEnter Student Marks:'))
            Dict[Roll]['M2']=int(input('\nEnter Student Marks:'))
    elif int(Choice)==2:
        Roll=int(input('Enter Rollno to search:'))
        if Roll in Dict:
            print('\nStudent Details:',Dict[Roll])
        else:
            print('\nError: Roll num does not exist:')
    elif int(Choice)==3:
        Roll=int(input('Enter rollno to remove:'))
        if Roll in Dict:
            del Dict[Roll]
            print('\nStudent Detials is succesfully Removed',)
        else:
            print('\nError: Roll num does not exist:')
    elif int(Choice)==4:
        print('  ||================================||')
        print('  ||--------------------------------||')
        print('  ||Thankyou for using our system ☺♥||')
        print('  ||--------------------------------||')
        print('  ||================================||')
        break
    else:
        print('\nPlease provide a valid input')
                
        
        

    
