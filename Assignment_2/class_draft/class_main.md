classDiagram

User <|-- Student
User <|-- Instructor
User <|-- Admin

User "1"--"1" View

Student "1"--"1" GameView
Instructor "1"--"1" GameView

GameController "1"--"1" GameView

Controller <|-- GameController
Controller <|-- DashboardController

DashboardController "1"--"1" View
Controller "1"--"1" LoginForm
Controller "1"--"*" DataElement
GameController "1"--"*" Course

Course "1"--"*" Stage
CourseMaterials "*"--"1" Stage
Assignment "*"--"1" Stage
Puzzles "*"--"1" Stage

UserInfo <|-- StudentInfo
UserInfo <|-- InstructorInfo
UserInfo <|-- AdminInfo

Database "1"--"*" DataElement
DataElement <|-- CourseMaterials
DataElement <|-- Assignment
DataElement <|-- Puzzles
DataElement <|-- UserInfo

class User{
+int id
+String name
+String type
}

class Student{
+int stage
+int level
+startNewGame()
+continueFromlastCheckpoint()
}

class Instructor{
+String course
+sendMessageToStudent()
+approveYearMarks()
+editCourseContent()
}

class Admin{
+int active_ticket_id
+manage()
+authenticate()
}

class LoginForm{
+String enteredID
+String enteredPassword
+login()
+forgotPassword()
}

class View{
+String cssStyle
+String HTMLForm
+sendCredendtialsToController()
}

class DashboardController{
+validateData()
+render()
}

class GameController{
+capture_action()
+loadFigures()
}

class UserInfo{
+int age
}

class StudentInfo{
+int age
}


class InstructorInfo{
+int age
}


class AdminInfo{
+int age
}

class Course{
+String course_code
+String Name
+int intructor_code
}


class Stage{
 
}


class CourseMaterials{
+String courseContent
}

class Puzzles{
 
}

class Assignment{
 
}

class DataElement{
+studentID
+instructorID
+getID()
+getName()
}

class Database{
+table StudentsTakingCourse
+table instructors

}

class GameView{
+String usertype    
+displayFigures()
}