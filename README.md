"# task-4-Java-File-I-O-Notes-App-" 

#  NotesApp – Java File I/O Project

##  Task 4: Java File I/O – Notes App

###  Objective:
Create a **text-based Notes Manager** using Java File I/O that allows users to **write** and **read** notes from a file using `FileWriter`, `FileReader`, or `BufferedReader`.

---

##  Tools Used
- Java (JDK 21)
- Eclipse IDE
- Terminal / Console (for input/output)

---

##  Project Structure
NotesApp/
├── src/
│ └── NotesApp.java


---

##  Flow of Code (How it Works)

### 1. **Program Starts**
- The program displays a simple **menu**:
  - 1. Write Note
  - 2. Read Notes
  - 3. Exit

### 2. **Write Note**
- User enters a note.
- `FileWriter` is used in **append mode** to save the note into `notes.txt`.
- Each note is written on a **new line** using `System.lineSeparator()`.

### 3. **Read Notes**
- If the file `notes.txt` exists:
  - It reads all the notes using `BufferedReader`.
  - Displays each note with a `-` bullet.
- If file doesn't exist:
  - Message is shown: “No notes found.”

### 4. **Exit**
- Program exits cleanly.

---

##  File I/O Used

###  Writing to File:
```java
FileWriter writer = new FileWriter(FILE_NAME, true);
writer.write(note + System.lineSeparator());



