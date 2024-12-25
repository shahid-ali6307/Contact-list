# Contact-list
contact = {}

while True :
	print("\n contact book app")
	print("press 1 for creating contact")
	print("press 2 for viewing contact")
	print("press 3 for deleting contact")
	print("press 4 for searching contact")
	print("press 5 for counting contact")
	print("press 6 for exiting contact")
	print("press 7 for nothing")
	
	
	choice=int(input("Enter the operstion you want to perform"))
	
	
	if (choice==1):
		
		name=input("Enter name : ")
		if name in contact:
			print(" this contact exists already")
			
		else:
			mobile=int(input("Enter mobile number : "))
			email=input("Enter email address : ")
			contact[name]={'mobile':mobile,'email':email}
			print("the new contact is added succesfully")
	
	
	elif(choice==2):
		name=input("Enter name you eant to see ")
		if name in contact:
			print("name : " , name ,  "number  : " ,number ,"E mail : " , email )
			
		else:
			print("contact does not exist")
			
	elif(choice==3):
		name = input("Enter the contact you want to update")
		
		if name in contact:
			mobile=input("enter the name")
			mail=input("enter the e mail")
			contact[name]={'age':int(age),'email':email,'mobile':mobile}
			print("your contact updated succesfully")
			
			
		else:
			print("the contact does not exist in contact")
			
			
	elif(choice==4):
		name=input("Enter name you want to search")
		
		if name in contact:
			print("this contact exists in your contact")
			print("name : " , name ,  "number  : " ,number ,"E mail : " , email )
			
		else:
			print("this contact does not exist in contact")
	elif(choice==5):
			print("total contact in the list is " , len(contact))
			
	else:
			print("Do you want to exit....?")
			take=input("yes or no")
			if take=='yes':
				print("you have been exited from program successfully")
				break
