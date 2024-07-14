# Project: Student-Management-System
# This is a project where we analyze student data.

def calculate_highest_in_maths(student_list):
    highest_score_in_maths = 0
    highest_score_in_maths_name = ""
    region_of_the_student = ""
    
    for student in student_list:
        if (student.get("maths") > highest_score_in_maths):
            highest_score_in_maths = student.get("maths")
            highest_score_in_maths_name = student.get("name")
            region_of_the_student = student.get("region")
    print(f"The highest scorer in maths is {highest_score_in_maths} by {highest_score_in_maths_name} from {region_of_the_student}")
    
def calculate_highest_in_science(student_list):
    highest_score_in_science = 0
    highest_score_in_science_name = ""
    region_of_the_student = ""
    
    for student in student_list:
        if (student.get("science") > highest_score_in_science):
            highest_score_in_science = student.get("science")
            highest_score_in_science_name = student.get("name")
            region_of_the_student = student.get("region")
    print(f"The highest scorer in science is {highest_score_in_science} by {highest_score_in_science_name} from {region_of_the_student}")

def calculate_highest_in_social(student_list):
    highest_score_in_social = 0
    highest_score_in_social_name = ""
    region_of_the_student = ""
    
    for student in student_list:
        if (student.get("social") > highest_score_in_social):
            highest_score_in_social = student.get("social")
            highest_score_in_social_name = student.get("name")
            region_of_the_student = student.get("region")
    print(f"The highest scorer in social is {highest_score_in_social} by {highest_score_in_social_name} from {region_of_the_student}")

student_1 = {
    "maths": 45,
    "social": 62,
    "science": 95,
    "name": "tanmay",
    "region": "bangalore"
}
student_2 = {
    "maths": 74,
    "social": 83,
    "science": 96,
    "name": "Dheeraj",
    "region": "mysore"
}
student_3 = {
    "maths": 79,
    "social": 90,
    "science": 98,
    "name": "sooraj",
    "region": "chamarajanagar"
}

student_list = [student_1, student_2, student_3]
calculate_highest_in_maths(student_list)
calculate_highest_in_science(student_list)
calculate_highest_in_social(student_list)
