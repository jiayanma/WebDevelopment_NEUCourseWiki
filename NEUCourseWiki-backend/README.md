# NEU Course Wiki Backend

This is the NEU course Wiki Backend. We use MongoDB for the local database,express for the connection and GraphQL for the api. 

the backend includes four parts.

- Courses
- Instructors
- Reviews
- Projects



## DataBase

#### Courses

Courses include four parts of information.

- course_id
- name
- introduction
- timeline

#### Reviews

Reviews include nine parts of information.

- course_id
- user_id
- content
- creationDate
- rating_difficultiness
- rating_usefulness
- semester
- instructor
- isRecommended

#### Instructors

Courses include two parts of information.

- name
- courses(which is a list to save all the courses taught by the instructor)

#### Projects

Projects include five parts of information

- course_id
- semester
- instructor
- description
- link



## API

####        Courses

- addCourse
- updateCourse
- deleteCourse
- getCourseById

#### 		Instructors

- addInstructor
- updateInstructor
- getAllInstrutors
- getInstructorsByCourseId

#### 		Projects

- addProjects
- getProjectsByCourseId
- getProjectsByInstructor
- getProjectsBySemester

#### 		Reviews

- addReview
- deleteReview
- getReviewsByCourse
- getReviewsByUser
- getReviewsBySemester
- getReviewsByInstructor



## Route

The backend has four routes.

- http://localhost:5000/api/v1/instructors
- http://localhost:5000/api/v1/review
- http://localhost:5000/api/v1/projects
- http://localhost:5000/api/v1/course

To test all the routes and api, you can use GraphiQL to test.

![](README.assets/grapgql.png)

