classDiagram

User <|-- Student
User <|-- Instructor
User <|-- Admin

User "1"--"1" View

Student "1"--"1" GameView

GameController "1"--"1" GameView

Controller <|-- GameController
Controller <|-- DashboardController

DashboardController "1"--"1" View
Controller "1"--"1" LoginForm
Controller "1"--"*" DataElement
DataElement <|-- Course

Course "1"--"*" Stage
StageMaterial "*"--"1" Stage
Puzzles "*"--"1" Stage

UserInfo <|-- StudentInfo
UserInfo <|-- InstructorInfo
UserInfo <|-- AdminInfo

Database "1"--"*" DataElement
DataElement <|-- StageMaterial
DataElement <|-- Puzzles
DataElement <|-- UserInfo

class User{
+int id
+String name
+String type
}

class Student{
+startStartGame()
+continueFromlastCheckpoint()
+preveiwCurrentState()
+preveiwCurrentLevel()
}

class Instructor{
+sendMessageToStudent()
+approveYearMarks()
+editCourseContent()
+showActiveCourse()
}

class Admin{
+displayActiveticketID()
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
+course
+stage
+stageMaterials
+puzzle
+getStageObject()
+getStageMaterialObject()
+getPuzzleObject()
+startGame()
+pause()
+solvePuzzle(answer)
+capture_action()
+loadFigures()
}

class UserInfo{
+int ID
}

class StudentInfo{
+int stage
+int level
+getCourseCode()
+updatScore(puzzle_id, score)
+MultipyScoreByDecayingFactor(puzzle_id)
+nextStage()
}


class InstructorInfo{
+int activeCourse
}


class AdminInfo{
+int activeTicketID
}

class Course{
+course_code
+Name
+stage
+stageMaterials
+puzzle
+createStageObject(stage_id)
+createPuzzleObject(puzzle_id)
+createStageMaterials_object(m_id)
+intructor_code
+getStageobject(stage_id)
}


class Stage{
+puzzleObject
+stageMaterialsObject
+getPuzzleObject()
+getStageMaterialObject()
}


class StageMaterial{
+courseContent
}

class Puzzles{
isCorrect(answer) 
}


class DataElement{
+objectID
+getID()
+getName()
+getObject(ObjectType, code)
+delete()
}

class Database{
+table StudentsTakingCourse
+table instructors
+getDataElementObject(ObjectType, object_id)
+store(altered_data)

}

class GameView{
+stage
+stageMaterials
+Puzzle
+displayFigures()
+render(ViewType)
+maneuverGame()
+startPuzzle()
+restartStage()
+pause()
}
