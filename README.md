# Grumpy Old Professor's Course Management System

## Introduction

This is the documentation, explanation, community, etc. repository for the
Grumpy Old Professor's Course Management System. The GitHub Project
[Grumpy Old Professor's Course Management System](https://github.com/users/donald-f-ferguson/projects/9)
is the coordinating GitHub project.


## Course Management System Overview

| <img src="./system-overview.jpg"> |
|:---------------------------------:|
|        __System Overview__        |

There are two major subsystems in the overall system:
1. The _interactive system_ is a set of microservices and web UIs that enable students, 
TAs, instructors, etc. to read and update information, and accomplish tasks.
2. The _data insight system_ enables the instructor and TA to analyze data, create reports, etc.

The system in cloud based and relies on a set of cloud application and infrastructure.


| <img src="./interactive-system.jpg"> |
|:------------------------------------:|
|         __System Overview__          |

Several microservices and web UIs make up the interactive systems:
- Students and profiles manages basic student information.
- Courses and sections manages information about courses, sections of courses
and enrollments in courses. This microservice relies on a CourseWorks adaptor (not shown)
the provides read access to CourseWorks data.
- Teams and projects manages teams and students' participation in teams, and associated
presentations, documents, etc.
- Meetings and minutes enables meeting scheduling, recording attendance and documenting
minutes and actions.
- Comments and discussions enables thread discussions related to meetings, projects, etc.
- Course project management is a composites microservice that integrates the base services
into an overall system.
- There are two backends-for-frontends that adapt the APIs to the specific users and roles.
- There is a single page web application project that provides the user interface.

__Note:__ These are the current repositories for random work that has been done. We need to align with the
above classification and work efforts. This is mostly just been a random set of thoughts.
- UI/UX: https://github.com/donald-f-ferguson/course-management-ui.git
- Project/Teams: https://github.com/donald-f-ferguson/project-teams.git
- Core Person Information: https://github.com/donald-f-ferguson/person-info.git
- CourseWorks adaptor: https://github.com/donald-f-ferguson/courseworks-adaptor-service.git
- Core course management: https://github.com/donald-f-ferguson/core-course-management.git
- Coupon management: https://github.com/donald-f-ferguson/course-coupons.git

