# JASON's CoWorking Space ☕

A JavaFX desktop application for managing a co-working space — built with Java OOP principles, featuring room reservations, slot management, user accounts, and an admin dashboard.

---

## 🎥 Demo

> 👉 [See demo on LinkedIn](https://www.linkedin.com/posts/abdelazizadel_java-oop-desktopapp-activity-7340931457038581762-KlLQ)

---

## ✨ Features

### 👤 User
- **Account system** — Register, log in, and update personal info
- **Room reservations** — Book Teaching, General, or Formal rooms
- **Slot management** — Browse and select available time slots with live hour tracking
- **Color/preference selection** — Personalize your workspace experience
- **VIP membership** — Access exclusive perks and leaderboard rankings
- **Leaderboard** — See top users across the space

### 🛠️ Admin
- **User management** — View and manage all registered users
- **Room & slot control** — Monitor and adjust room capacity and availability
- **Activity logging** — Full log of all system activity via `log.txt`
- **Multi-step admin flow** — Structured choice-based admin dashboard (Choice0–Choice6)

---

## 🧠 Tech Stack

| Layer | Details |
|---|---|
| Language | Java |
| GUI Framework | JavaFX (FXML) |
| Styling | CSS (`Style.css`) |
| Build Tool | Maven (`pom.xml`) |
| Architecture | OOP — MVC pattern (Controllers / Rooms / DataBase / Functionality) |
| Persistence | File handling (`data.txt`, `slots.txt`, `capacity.txt`, `log.txt`) |

---

## 🗂️ Project Structure

```
src/main/java/JasonOOP/
├── Controllers/
│   ├── Admin/               # Admin multi-step flow controllers
│   ├── Login_Controller.java
│   ├── CreateAccount_Controller.java
│   ├── Room_Controller.java
│   ├── Slots_Controller.java
│   ├── Reservations_Controller.java
│   ├── Leaderboard_Controller.java
│   └── ...more controllers
├── Rooms/
│   ├── ROOM.java            # Base room class
│   ├── General_Room.java
│   ├── Teaching_Room.java
│   └── Meeting_Room.java
├── DataBase/
│   ├── slots.java
│   ├── users.java
│   ├── userSetting.java
│   └── log.java
├── Functionality/
│   ├── LiveHourCounter.java
│   └── SceneSwitch.java
└── Main.java

src/main/resources/com/example/gui/
├── Login.fxml / Welcome.fxml / CreateAccount.fxml
├── General.fxml / Formal.fxml / Instructor.fxml
├── Slots.fxml / SlotsDate.fxml / Reservations.fxml
├── Leaderboard.fxml / Room.fxml / UpdateInfo.fxml
├── Admin/                   # Admin FXML screens
└── css/Style.css
```

---

## 🚀 Getting Started

### Prerequisites
- Java 17+
- Maven
- IntelliJ IDEA (recommended) or any IDE with JavaFX support

### Run
```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/jason-coworking-space

# Navigate into the project
cd jason-coworking-space

# Run with Maven
./mvnw javafx:run
```

Or open in **IntelliJ IDEA** → Import as Maven project → Run `Main.java`

---

## 📄 License

Built as an academic project. Feel free to explore and build on it!
