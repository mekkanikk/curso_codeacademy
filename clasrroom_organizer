import itertools
from roster import student_roster
# Import modules above this line

student_roster_iterator = iter(student_roster)

student_roster_places = itertools.combinations(student_roster_iterator, 2)

from classroom_organizer import ClassroomOrganizer 

new_student = ClassroomOrganizer()
student_roster_iterator = iter(student_roster)
print("task 1")
print("The full student roster (dictionary):")
for each_student in range(len(student_roster)):
  print(next(student_roster_iterator))

print()
print("task 3")
print("Each student by 'first' name one at a time, alphabetically:")

for each_name in new_student.sorted_names: 
  print(each_name[:-1])

print()
print("The student names, alphabetically as a list:")
print(new_student.sorted_names)
print()
print("Each student by first name and last initial one at a time:")
for each_student in new_student.sorted_names:
  print(each_student)

print()
print("task 4 - Two students combos possible")
two_students = new_student.two_students_combos()
print(two_students)

print()
#print(new_student.get_students_with_subject("Math"))
#print(new_student.get_students_with_subject("Science"))
print("task 5: favorite subject is Math or Science")
math_science_list = list(itertools.chain(new_student.get_students_with_subject("Math"), new_student.get_students_with_subject("Science")))
print(math_science_list)
print()
print("task 5: combos of tables of four.")
math_science_fours = list(itertools.combinations(math_science_list, 4))
print(math_science_fours)

print()
print("task 6:")
print("Each student and their favorite animal")
for item in sorted(new_student.get_student_name_animal()):
  print("{} - {}".format(item[0], item[1]))

print()
print("task 6: student name, age, height")
for item in sorted(new_student.get_students_with_info()):
  print('{}: {} years, {}"'.format(item[0], item[1], item[2]))
