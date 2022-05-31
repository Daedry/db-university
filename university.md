# DB UNIVERSITY

## 

##

## STUDENTS

- id :                                                PK NOT NULL UNIQUE INDEX
- name :                                          VARCHAR(40) NOT NULL
- lastname :                                     VARCHAR(40) NOT NULL
- freshman :                                    VARCHAR(30) NOT NULL
- email :                                          VARCHAR(60) NOT NULL
- date :                                            DATETIME NOT NULL
- address :                                       VARCHAR(50) NULL
- country :                                       VARCHAR(50) NULL
- phone_number :                           VARCHAR(50) NOT NULL
- documentation :                           VARCHAR(50) NOT NULL
- ?department_id? :                         
- ?degree_courses_id? :
- ?course_id? :
- ?examination_appeal_id? :
- ?exam_taken_id? :
- ?examination_appeals_id? :

## TEACHERS

- id :                                                PK NOT NULL UNIQUE INDEX
- name :                                          VARCHAR(40) NOT NULL
- lastname :                                     VARCHAR(40) NOT NULL
- email :                                           VARCHAR(60) NOT NULL
- date :                                            DATETIME NULL          
- phone_number :                           VARCHAR(50) NULL
- ?course_id? :
- ?exam_id? :

## DEPARTMENTS

- id :                                              PK NOT NULL UNIQUE INDEX
- name :                                        VARCHAR(40) NOT NULL
- address :                                     VARCHAR(50) NOT NULL
- phone_number :                         TINYINT NOT NULL
- description :                               TEXT NOT NULL
- website :                                     VARCHAR(50) NOT NULL
- ?degree_courses_id? :

## DEGREE_COURSE

- id :                                              PK NOT NULL UNIQUE INDEX
- name :                                        VARCHAR(40) NOT NULL
- code :                                         SMALLINT NOT NULL
- year :                                          YEAR NOT NULL
- principal_subject :                      VARCHAR(100) NOT NULL            
- description :                               TEXT NOT NULL
- closed_number :                         TINYINT NOT NULL
- website :                                     VARCHAR(50) NOT NULL
- ?department_id? :
- ?teacher_id? :

## COURSE

- id :                                              PK NOT NULL UNIQUE INDEX
- name :                                        VARCHAR(40) NOT NULL
- code :                                         SMALLINT NOT NULL
- year :                                          YEAR NOT NULL
- subject :                                      VARCHAR(40) NOT NULL
- description :                               TEXT NOT NULL
- credits :                                      TINYINT NOT NULL
- ?teacher_id? :                                   
- ?degree_courses_id? :

## EXAMINATION_APPEALS

- id :                                                  PK NOT NULL UNIQUE INDEX
- name :                                            VARCHAR(40) NOT NULL
- code :                                             SMALLINT NOT NULL   
- year :                                              YEAR NOT NULL
- subject :                                          VARCHAR(40) NOT NULL
- date :                                               DATETIME NOT NULL
- description :                                    TEXT NOT NULL
- credits :                                           TINYINT NOT NULL

- ?courses_id? :

## EXAMS

- id :                                                    PK NOT NULL UNIQUE INDEX
- name :                                              VARCHAR(40) NOT NULL
- code :                                               SMALLINT NOT NULL
- subject :                                           VARCHAR(40) NOT NULL
- date :                                                DATETIME NOT NULL
- vote :                                                TINYINT NOT NULL
- ?examination_appeals_id? :                
- ?degree_courses_id? :

## EXAMS_TAKEN

- id :                                                  PK NOT NULL UNIQUE INDEX
- name :                                            VARCHAR(40) NOT NULL
- subject :                                         VARCHAR(40) NOT NULL
- vote :                                              TINYINT NOT NULL
- date :                                               DATETIME NOT NULL
- credits :                                            TINYINT NOT NULL
- code :                                               TINYINT NOT NULL
- ?courses_id? :    
- ?teacher_id? :
