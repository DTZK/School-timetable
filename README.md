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

mon1=[]
tues1=[]
wed1=[]
thurs1=[]
fri1=[]

mon2=[]
tues2=[]
wed2=[]
thurs2=[]
fri2=[]

mon3=[]
tues3=[]
wed3=[]
thurs3=[]
fri3=[]

mon4=[]
tues4=[]
wed4=[]
thurs4=[]
fri4=[]

mon5=[]
tues5=[]
wed5=[]
thurs5=[]
fri5=[]

mon6=[]
tues6=[]
wed6=[]
thurs6=[]
fri6=[]

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

for counter in range (2):
    mon1.append(mon1)
    mon2.append(mon2)
    mon3.append(mon3)
    mon4.append(mon4)
    mon5.append(mon5)
    tues1.append(tues1)
    tues2.append(tues2)
    tues3.append(tues3)
    tues4.append(tues4)
    tues5.append(tues5)
    wed1.append(wed1)
    wed2.append(wed2)
    wed3.append(wed3)
    wed4.append(wed4)
    wed5.append(wed5)
    wed6.append(wed6)
    thurs6.append(thurs6)
    fri6.append(fri6)
    #chemistry as 1 st 2
    mon1[counter] = classes[0]
    tues3[counter] = classes[0]
    wed5[counter] = classes[0]
    # Physics 1st 2
    tues2[counter] = classes[1]
    wed4[counter] = classes[1]
    mon5[counter] = classes[1]
    fri6[counter] = classes[1]
    # Programming 1st 2
    tues1[counter] = classes[2]
    wed3[counter] = classes[2]
    mon4[counter] = classes[2]
    thurs6[counter] = classes[2]
    #Math 1st 2
    wed2[counter] = classes[3]
    mon3[counter] = classes[3]
    tues5[counter] = classes[3]
    # Bio 1st 2
    wed1[counter] = classes[4]
    mon2[counter] = classes[4]
    tues4[counter] = classes[4]

for counter in range (2,4):
    mon1.append(mon1)
    mon2.append(mon2)
    mon3.append(mon3)
    mon4.append(mon4)
    mon5.append(mon5)
    tues1.append(tues1)
    tues2.append(tues2)
    tues3.append(tues3)
    tues4.append(tues4)
    tues5.append(tues5)
    wed1.append(wed1)
    wed2.append(wed2)
    wed3.append(wed3)
    wed4.append(wed4)
    wed5.append(wed5)
    wed6.append(wed6)
    thurs6.append(thurs6)
    fri6.append(fri6)
    #Chemistry as last 2 periods
    mon2[counter] = classes[0]
    tues4[counter] = classes[0]
    fri6[counter] = classes[0]
    #Physics as last 2 periods
    mon1[counter] = classes[1]
    tues3[counter] = classes[1]
    #Programming as last 2
    tues2[counter] = classes[2]
    mon5[counter] = classes[2]
    #Math
    tues1[counter] = classes[3]
    mon4[counter] = classes[3]
    thurs6[counter] = classes[3]
    #Bio
    mon3[counter] = classes[4]
    tues5[counter] = classes[4]
    wed6[counter] = classes[4]
    #Study
    wed1[counter] = "Study"
    wed2[counter] = "Study"
    wed3[counter] = "Study"
    wed4[counter] = "Study"
    wed5[counter] = "Study"

for counter in range(0,4):
    thurs1.append(thurs1)
    thurs2.append(thurs2)
    thurs3.append(thurs3)
    thurs4.append(thurs4)
    thurs5.append(thurs5)
    mon6.append(mon6)
    tues6.append(tues6)
    fri1.append(fri1)
    fri2.append(fri2)
    fri3.append(fri3)
    fri4.append(fri4)
    fri5.append(fri5)
    thurs1[counter] = "Study"
    thurs2[counter] = "Study"
    thurs3[counter] = "Study"
    thurs4[counter] = "Study"
    thurs5[counter] = "Study"
    mon6[counter] = "Study"
    tues6[counter] = "Study"
    fri1[counter] = "Study"
    fri2[counter] = "Study"
    fri3[counter] = "Study"
    fri4[counter] = "Study"
    fri5[counter] = "Study"

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
