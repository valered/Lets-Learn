# Lets-Learn

Lets-Learn is a Java-based educational web application designed to support **language learning for children**, with particular attention to **young learners with migrant backgrounds** who may experience difficulties with the local language.

The project was developed as a **group university project** during the Bachelor’s degree, within the course *Human–Computer Interaction*, with a strong focus on **usability, accessibility, and learning through interaction**.

---

## 📌 Project Overview

Lets-Learn aims to help children acquire **basic vocabulary and simple sentence structures** through an interactive and visual learning experience.

The application is based on:
- **Word cards** associated with images
- **Audio playback** to support pronunciation
- **Interactive exercises** (association, translation, completion)
- **Immediate feedback** and corrections

The design choices were guided by HCI principles to make the learning process:
- intuitive
- engaging
- suitable for young users

---

## 🎯 Educational Goals

- Support early language acquisition
- Reduce linguistic barriers for children in multicultural contexts
- Encourage learning through **visual and auditory association**
- Provide a simple and guided user experience

---

## 🧱 Architecture & Technologies

**Backend**
- Java 8
- Java Servlets
- JDBC
- Maven (WAR packaging)

**Frontend**
- JSP
- HTML / CSS
- JavaScript
- Bootstrap

**Server**
- Apache Tomcat (or compatible servlet container)

---

## 📂 Project Structure

```text
Lets-Learn/
│
├── src/main/java/
│   ├── Classi/                  # Core application logic and models
│   │   ├── Argomento.java
│   │   ├── Card.java
│   │   ├── Database.java
│   │   ├── DatabaseEsercizi.java
│   │   └── DatabaseTeoria.java
│   │
│   └── Servlet/                 # Application controllers
│       ├── ServletEsercizi.java
│       ├── ServletCorrezione.java
│       ├── ServletDizionario.java
│       └── (other exercise-related servlets)
│
├── src/main/webapp/
│   ├── WEB-INF/
│   │   ├── web.xml               # Application configuration
│   │   ├── General/              # Main JSP pages
│   │   ├── Header/               # Shared UI components
│   │   └── Partials/             # Exercise-specific JSP fragments
│   │
│   ├── bootstrap-*               # Bootstrap libraries
│   ├── customcss/                # Custom styles
│   ├── javascript/               # Interactive exercise scripts
│   └── Immagini/                 # Visual learning assets
│
├── pom.xml                       # Maven configuration
└── README.md
```

---

## ⚙️ Requirements

- Java 8 or higher
- Maven
- Apache Tomcat (or equivalent servlet container)
- Relational database (for exercises, theory, and vocabulary)

---

## ▶️ How to Run

1. Configure the database connection in the corresponding Database classes

2. Build the project using Maven:
```text
mvn clean package
```

3. Deploy the generated WAR file on a servlet container (e.g. Tomcat)

4. Open the application in a browser:
```text
http://localhost:8080/Lets-Learn
```

---

## 🧠 Human–Computer Interaction Focus

Special attention was given to:

- clarity of navigation
- minimal cognitive load
- visual feedback
- consistency across exercises

The interface and interaction flow were designed to be child-friendly and accessible, in line with the objectives of the HCI course.

---

## 🧪 Notes

- The project was developed for educational purposes
- Emphasis is placed on usability and learning effectiveness rather than production deployment
- The application can be extended with additional languages or exercise types
