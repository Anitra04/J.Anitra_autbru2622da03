#
def sort_students(student_list):
    # Sort the student list based on CGPA in descending order
    sorted_students = sorted(student_list, key=lambda student: student['cgpa'], reverse=True)
    return sorted_students

# Define some sample student data
students = [
    {'name': 'ganeshkumar', 'roll number': 'A123', 'cgpa': 3.8},
    {'name': 'logesh', 'roll number': 'B456', 'cgpa': 3.5},
    {'name': 'mohan', 'roll number': 'C789', 'cgpa': 3.9},
    # Add more students here
]

# Test the sort_students function
sorted_students = sort_students(students)

# Print the sorted list of students
for student in sorted_students:
    print(f"Name: {student['name']}, Roll Number: {student['roll number']}, CGPA: {student['cgpa']}")