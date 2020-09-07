# covid19-assessment-tool
#covid 19
print('note: This is an assessment tool, not a testing tool')

prompt = '\nPlease press any key to continue '
while True: 
    name = input(prompt)
    break 
    
print('\nkindly provide the correct information')
print('\nShall we begin?')
input('Strike enter to continue')

#user information
name = input('\nFull name: ')
gender = input('Gender: ')
age = input('Age: ')
address = input('Address: ')
location = input('State: ')
local_government = input('LGA: ')
country = input ('Country ')
Telephone = input('Phone number: ')

#covid19 symptoms 
print("\nInput either 'yes' or 'no'")
input('Strike enter to continue...')
symptom_1 = 'Do you travelled in the last 25 days to a covid19 infected country? '
while True: 
    symp_1 = input (symptom_1)
    if symp_1 == 'yes':
        break  
    elif symp_1 == 'no':
        break 
    else: 
        print("Please input 'yes' or 'no'")
  
        
symptom_2 = 'Are you feeling feverish? '
while True: 
    symp_2 = input (symptom_2)
    if symp_2 == 'yes':
        break  
    elif symp_2 == 'no':
        break 
    else: 
        print("Please input 'yes' or 'no'")
        
symptom_3 = 'Do you have sore throat? '
while True: 
    symp_3 = input (symptom_3)
    if symp_3 == 'yes':
        break  
    elif symp_3 == 'no':
        break 
    else: 
        print("Please input 'yes' or 'no'")
        
symptom_4 = 'Are you coughing? '
while True: 
    symp_4 = input (symptom_4)
    if symp_4 == 'yes':
        break  
    elif symp_4 == 'no':
        break 
    else: 
        print("Please input 'yes' or 'no'")
        
symptom_5 = 'Is your temperature above 37degree celsius? '
while True: 
    symp_5 = input (symptom_5)
    if symp_5 == 'yes':
        break  
    elif symp_5 == 'no':
        break 
    else: 
        print("Please input 'yes' or 'no'")
        
symptom_6 = 'Do you attend any social gathering? '
while True: 
    symp_6 = input (symptom_6)
    if symp_6 == 'yes':
        break  
    elif symp_6 == 'no':
        break 
    else: 
        print("Please input 'yes' or 'no'")

#answer
answer = []
answer.append(symptom_1)
answer.append(symptom_2)
answer.append(symptom_3)
answer.append(symptom_4)
answer.append(symptom_5)
answer.append(symptom_6)

#result
answers = answer.count('yes')
if answers > 3:
    print('\nYou might have contracted the COVID19, please kindly call NCDC!')
else: 
    print (f"\nCongratulations, {name.title()} You are COVID19 free")
