# School-timetable
classes =["Chem", "Physics", "Programming", "Math", "Bio"]
teachers_teaching_length = []
teachers_name = []
main_subject = []
numberofteachers = int(input("How many teachers are there"))
required_chem_teachingperiod = 0
required_physics_teachingperiod = 0
required_programming_teachingperiod = 0
required_math_teachingperiod = 0
required_bio_teachingperiod = 0
current_mathperiods= 12
current_physicsperiods = 12

mon1=["PSHE", "Chem", "Chem", "Study"]
tues1=["PSHE", "PE", "Physics", "Physics"]
wed1=["PSHE","Programming", "Programming", "Study"]
thurs1=["PSHE", "Math", "Math", "Study"]
fri1=["PSHE", "PE", "Bio", "Bio"]

mon2=["PSHE","Bio", "Bio","Study"]
tues2=["PSHE","PE", "Chem", "Chem"]
wed2=["PSHE", "Physics", "Physics","Study"]
thurs2=["PSHE", "Programming", "Programming", "Study"]
fri2=["PSHE", "PE", "Math", "Math"]

mon3=["PSHE", "Math", "Math", "Study"]
tues3=["PSHE", "PE", "Bio", "Bio"]
wed3=["PSHE","Chem", "Chem", "Study"]
thurs3=["PSHE","Physics", "Physics","Study"]
fri3=["PSHE", "PE","Programming", "Programming"]

mon4=["PSHE","Programming", "Programming", "Study"]
tues4=["PSHE", "PE", "Math", "Math"]
wed4=["PSHE", "Bio", "Bio","Study" ]
thurs4=["PSHE","Chem", "Chem", "Study" ]
fri4=["PSHE", "PE","Physics", "Physics"]

mon5=["PSHE","Physics", "Physics", "Study" ]
tues5=["PSHE", "PE","Programming", "Programming"]
wed5=["PSHE", "Math", "Math", "Study"]
thurs5=["PSHE", "Bio", "Bio","Study" ]
fri5=["PSHE", "PE", "Chem", "Chem"]

mon6=["Physics", "Study", "PSHE", "Physics"]
tues6=["Programming", "Programming", "PSHE", "PE"]
wed6=["Math","Study", "PSHE","Math" ]
thurs6=["Bio", "Study", "PSHE", "Bio"]
fri6=["Chem", "Chem", "PSHE", "PE"]

while numberofteachers< 0 or numberofteachers>10:
    print("Invalid number. Must be at least 0 or at max 10")
    numberofteachers= int(input("How many teachers are there"))

for counter in range(0,numberofteachers):
    teachers_name.append(teachers_name)
    main_subject.append(main_subject)
    teachers_teaching_length.append(teachers_teaching_length)
    print("These are the subjects", classes)
    teachers_name[counter] = input("Please enter the name of a teacher")
    teachers_teaching_length[counter] = int(input("Enter the number of periods that he or she wil be having per month "))
    main_subject[counter]= input("Which of the subject above that he or she wil be teaching. Please type the exact same words")
    if main_subject[counter] == "Chem":
        required_chem_teachingperiod = required_chem_teachingperiod +1
    if main_subject[counter] == "Physics":
        required_physics_teachingperiod = required_physics_teachingperiod +1
        while required_physics_teachingperiod<0 or required_physics_teachingperiod<12:
                print("This requirement period is not between 0 or 12. Please input again")
                teachers_teaching_length[counter] = int(input("Please enter again for Physics"))
    if main_subject[counter] == "Programming":
        required_programming_teachingperiod = required_programming_teachingperiod +1
    if main_subject[counter]=="Math":
        required_math_teachingperiod = required_math_teachingperiod+1
        while required_math_teachingperiod<0 or required_math_teachingperiod<12:
            print("This requirement period is not between 0 or 12. Please input again")
            teachers_teaching_length[counter] = int(input("Please enter again for Math"))
    if main_subject[counter] == "Bio":
        required_bio_teachingperiod = required_bio_teachingperiod+1

print("-This is for Class 1-")
print("Monday", mon1)
print("Tuesday", tues1)
print("Wednesday", wed1)
print('Thursday', thurs1)
print("Friday", fri1)
print("")

print("-This is for Class 2-")
print("Monday", mon2)
print("Tuesday", tues2)
print("Wednesday", wed2)
print('Thursday', thurs2)
print("Friday", fri2)
print("")

print("-This is for Class 3-")
print("Monday", mon3)
print("Tuesday", tues3)
print("Wednesday", wed3)
print('Thursday', thurs3)
print("Friday", fri3)
print("")

print("-This is for Class 4-")
print("Monday", mon4)
print("Tuesday", tues4)
print("Wednesday", wed4)
print('Thursday', thurs4)
print("Friday", fri4)
print("")

print("-This is for Class 5-")
print("Monday", mon5)
print("Tuesday", tues5)
print("Wednesday", wed5)
print('Thursday', thurs5)
print("Friday", fri5)
print("")

print("-This is for Class 6-")
print("Monday", mon6)
print("Tuesday", tues6)
print("Wednesday", wed6)
print('Thursday', thurs6)
print("Friday", fri6)
print("")
