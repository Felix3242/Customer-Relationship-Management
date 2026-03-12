# 🏢 Customer Relationship Management System
A Java Swing desktop application for managing client relationships, assignments, and team coordination with Firebase real-time synchronization. Built for telMAX Sales Operations with role-based access control for efficient lead management and assignment tracking.

## Features
- User authentication with secure email/password login
- Role-based dashboards for admins and sales representatives
- Client management with search and CSV import functionality
- Assignment tracking and completion workflows
- Real-time data synchronization with Firebase Realtime Database
- Custom Java Swing UI with intuitive navigation

## Tech Stack
- **Language**: Java 8+
- **GUI**: Java Swing
- **Database**: Firebase Realtime Database
- **Build Tool**: Gradle
- **Dependencies**: Firebase Admin SDK, JDatePicker (`org.jdatepicker:jdatepicker`)
- **Gradle** (build system)

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
## Setup & Running

### Prerequisites

- Java 8 or higher
- [Gradle](https://gradle.org/) (or use the included Gradle wrapper)
- A Firebase project with a Realtime Database and a service account key

### Firebase Setup

1. Go to [Firebase Console](https://console.firebase.google.com/), create a project, and enable Realtime Database.
2. Download your `serviceAccountKey.json` and place it in:
   - `app/src/main/resources/serviceAccountKey.json`

### Build & Run

**From the command line:**

```sh
cd app
./gradlew build
```

**To run the app:**

```sh
./gradlew run
```

**To create an executable JAR:**

```sh
./gradlew jar
```

The JAR will be in `app/build/libs/`. You can double-click it (if Java is installed and associated with `.jar` files) or run:

```sh
java -jar build/libs/app.jar
```

## Usage

- **Login**: Use your email and password to log in.
- **Admin Dashboard**: Add clients, assign clients, and view all clients.
- **Rep Dashboard**: View assigned clients and mark assignments as complete.
- **Import Clients**: Use the "Add Clients By CSV" feature to bulk import clients.

## Code Style & Contribution

- Code is organized by feature/component.
- Comments and JavaDoc are provided for clarity.
- Contributions are welcome! Please fork and submit a pull request.


---

**Authors:**  
[@AP0tat0](https://github.com/AP0tato)
[@PriSey](https://github.com/PriSey)
[@Dumplingbob](https://github.com/Dumplingbob)
[@Felix3242](https://github.com/Felix3242)


