# DB UNIVERSITY

## 

##

## STUDENTS

- id :
- name :
- lastname :
- freshman :
- email :
- date :
- address :
- country :
- phone_number :
- documentation :
- ?department_id? :
- ?degree_courses_id? :
- ?course_id? :
- ?examination_appeal_id? :
- ?exam_taken_id? :
- ?examination_appeals_id? :

## TEACHERS

- id :
- name :
- lastname :
- email :
- date :
- address :
- phone_number :
- ?course_id? :
- ?exam_id? :

## DEPARTMENTS

- id :
- name :
- address :
- phone_number :
- description :
- website :
- ?degree_courses_id? :

## DEGREE_COURSES

- id :
- name :
- code :
- year :
- subject :
- description :
- credits :
- closed_number :
- website :
- ?department_id? :
- ?teacher_id? :

## COURSES

- id :
- name :
- code :
- year :
- subject :
- description :
- credits :
- ?teacher_id? :
- ?degree_courses_id? :

## EXAMINATION_APPEALS

- id :
- name :
- code :
- year :
- subject :
- date :
- description :
- credits :

- ?courses_id? :

## EXAM

- id :
- name :
- code :
- subject :
- date :
- vote :
- ?examination_appeals_id? :
- ?degree_courses_id? :

## EXAMS_TAKEN

- id :
- name :
- subject :
- vote :
- date :
- ?courses_id? :
- ?teacher_id? :
