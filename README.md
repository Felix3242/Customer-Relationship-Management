# Customer Relationship Management System
A Java Swing desktop CRM for managing client relationships and team assignments with Firebase real-time sync. Built for telMAX Sales Operations with role-based access control.

## Features
- Role-based dashboards for admins and sales reps
- Client management with search and CSV bulk import
- Assignment tracking and completion workflows
- Firebase real-time data synchronization
- Secure email/password authentication

## Tech Stack
- **Language**: Java 8+
- **GUI**: Java Swing
- **Database**: Firebase Realtime Database
- **Build Tool**: Gradle
- **Dependencies**: Firebase Admin SDK, JDatePicker

## Project Structure
```
app/
  src/
    main/
      java/com/athabasca/
        App.java            # Entry point
        Login.java          # Login window
        Dashboard.java      # Main dashboard
        AddClient.java      # Add clients (form & CSV)
        AssignClient.java   # Assign clients to reps
        CheckAssignments.java # View/complete assignments
        ClientList.java     # View/search clients
        Session.java        # User session management
        DatabaseUtil.java   # Firebase database helper
        FileHelper.java     # File read/write utilities
        ... (other helpers and components)
      resources/
        serviceAccountKey.json # Firebase credentials
  build.gradle.kts
```
## Getting Started
**Prerequisites**: Java 8+, Gradle, Firebase project with Realtime Database

### Firebase Setup
- Create a project in Firebase Console and enable Realtime Database
- Download serviceAccountKey.json and place it in app/src/main/resources/

### Build & Run
```sh
cd app
./gradlew build
./gradlew run
```

To create an executable JAR:
```sh
./gradlew jar
java -jar build/libs/app.jar
```

---

**Authors:**  
[@AP0tat0](https://github.com/AP0tato)
[@PriSey](https://github.com/PriSey)
[@Dumplingbob](https://github.com/Dumplingbob)
[@Felix3242](https://github.com/Felix3242)


