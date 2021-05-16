Num = int(input('Please Enter Number Of Grades: '))

grades = []

# append grades
for i in range(1, Num + 1, 1):
    print('Grade ', i)
    grade = int(input('Please Enter Grade: '))
    grades.append(grade)

print(grades)

# find average
sum = 0
for i in range(0, Num, 1):
    sum += grades[i]
    avrg = sum / Num
print('Grades Avrage is: ', avrg)

# sort Array

for i in range(0, Num - 1, 1):
    for i in range(0, Num - 1, 1):
        if grades[i] < grades[i + 1]:
            swp = grades[i]
            grades[i] = grades[i+1]
            grades[i+1] = swp
print('sorted grade from heighest Num to lowest: ',grades)
# print('sorted Grades using sort function: ', sorted(grades)) # this fastest option to make sort array

