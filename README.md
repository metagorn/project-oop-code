ความเป็นมา
```
    เนื่องจากว่าห้องสมุดมีการลงทะเบียนยืมโน๊ตบุ๊ค แต่ไม่รู้ว่าใครยืมเครื่องไหนไปแล้วบ้างก็เลยจึงสร้างโปรแกรมนี้ขึ้นมา
```
วัตถุประสงค์ของโปรแกรม
```
    อยากรู้ว่าใครยืมบ้าง โดยการ กรอกรหัสนศ.,ชื่อ-นามสกุล,รุ่นโน๊ตบุ๊ค,ระยะเวลา

```
Class Diagram
```mermaid
classDiagram
  class Add{
    -Adddata()
}
  class Admin{
    +String studentid
    +String studentname
    +String NotebookID
    +String NotebookName
    +String date
    -loadfile()
    -savefile()
  }
  class Notebook{
    +string NotebookID
    +string NotebookName
   }
  class NotebookList{
    +Student student
    +Notebook notebook
    +DateTime date
   }
  class Notebooks{
    +new Notebook
    -getAllNotebooks()
   }
  class Student{
    +string studentid
    +string name
   }
   Add <|-- Admin
   Add <|-- Notebook
   Admin <|-- Student
   Admin <|-- NotebookList
   Admin <|-- Notebooks

```
ชื่อผู้พัฒนา
```
นาย เมธากร สิงห์คาน
```