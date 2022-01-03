```mermaid
classDiagram


User <|-- Student
User <|-- Instructor
User <|-- Admin


User -- LoginForm

DashboardController -- LoginForm
DashboardController -- UserInfo

DataElement <|-- UserInfo

Database -- DataElement

```
