# Lost and Found Portal

<img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=180&section=header&text=Lost+and+Found+Portal&fontSize=42&fontColor=fff&animation=twinkling&fontAlignY=32&desc=Full-Stack+Campus+Lost+and+Found+Management+System&descAlignY=62&descSize=16" />

<div align="center">

  <img src="https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white" alt="Java"/>
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" alt="Spring Boot"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white" alt="MySQL"/>
  <img src="https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white" alt="HTML5"/>
  <img src="https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white" alt="CSS3"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black" alt="JavaScript"/>

  <br/><br/>

  <a href="https://github.com/ArunkumarValandas/lost-and-found">
    <img src="https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub Repository"/>
  </a>

</div>

---

## About the Project

The **Lost and Found Portal** is a full-stack web application designed to digitize and simplify the process of reporting, searching for, and claiming lost items within a college campus.

Instead of relying on notice boards or word of mouth, students and staff can use this platform to report lost or found belongings, browse available listings, and submit claims to help reunite owners with their items.

The project uses **Java, Spring Boot, MySQL, HTML, CSS, and JavaScript** to provide a web-based solution for campus lost-and-found management.

---

## Features

- **Report Lost Items** — Submit details about missing belongings.
- **Report Found Items** — Publish information about items found on campus.
- **Search and Filter** — Browse item listings using keywords and available filters.
- **User Authentication** — Login and registration for users.
- **Claim Requests** — Submit requests to claim found belongings.
- **Admin Dashboard** — Manage item listings and claim requests.
- **Responsive Interface** — Access the portal from desktop and mobile devices.
- **Centralized Management** — Keep lost-and-found information organized in one place.

---

## Tech Stack

| Layer | Technology |
|---|---|
| Backend | Java, Spring Boot |
| Frontend | HTML5, CSS3, JavaScript |
| Database | MySQL |
| ORM | Spring Data JPA, Hibernate |
| Build Tool | Maven |
| Version Control | Git, GitHub |
| IDE | VS Code, Eclipse |

---

## Project Architecture

The application follows a layered architecture:

- **Controller Layer:** Handles incoming HTTP requests.
- **Service Layer:** Contains application business logic.
- **Repository Layer:** Communicates with the database.
- **Model Layer:** Represents application entities.
- **Static Frontend:** Provides the user interface using HTML, CSS, and JavaScript.
- **Database Layer:** Stores user accounts, item listings, and claim information.

---

## Project Structure

```text
lost-and-found/
├── src/
│   └── main/
│       ├── java/
│       │   └── com/
│       │       └── example/
│       │           └── lostfound/
│       │               ├── controller/
│       │               ├── model/
│       │               ├── repository/
│       │               ├── service/
│       │               └── LostFoundApplication.java
│       │
│       └── resources/
│           ├── static/
│           │   ├── css/
│           │   ├── index.html
│           │   ├── login.html
│           │   ├── register.html
│           │   ├── item.html
│           │   ├── post.html
│           │   ├── my-claims.html
│           │   └── admin-claims.html
│           │
│           └── application.properties
│
├── pom.xml
└── README.md
```

*Note: Adjust the package and file names in this tree if your actual project structure differs.*

---

## Getting Started

### Prerequisites

Install the following before running the project:

- Java Development Kit (JDK) 17 or later
- Apache Maven
- MySQL 8 or later
- Git
- VS Code or Eclipse (recommended)

### 1. Clone the Repository

```bash
git clone https://github.com/ArunkumarValandas/lost-and-found.git
cd lost-and-found
```

Make sure the repository exists under your GitHub account and that its name matches the URL.

### 2. Create the Database

Log in to MySQL and execute:

```sql
CREATE DATABASE lostfound;
```

### 3. Configure Database Credentials

Open:

`src/main/resources/application.properties`

Configure the connection using your own database settings:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/lostfound
spring.datasource.username=YOUR_MYSQL_USERNAME
spring.datasource.password=YOUR_MYSQL_PASSWORD
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=false

server.port=8080
```

Replace the username and password with your actual MySQL credentials.

If you are using AWS RDS instead of a local MySQL installation, use your current RDS endpoint and valid database credentials.

**Security:** Do not commit real database passwords, JWT secrets, or other credentials to GitHub.

### 4. Build the Project

Run this command from the directory containing `pom.xml`:

```bash
mvn clean package
```

### 5. Run the Application

```bash
mvn spring-boot:run
```

### 6. Open the Website

Once the application starts successfully, visit:

**http://localhost:8080**

The application requires a working database connection to start successfully.

---

## How It Works

1. A user opens the Lost and Found Portal.
2. The user registers or logs in, where authentication is configured.
3. The user submits details of a lost or found item.
4. Other users browse and search the available listings.
5. A user submits a claim request for a relevant found item.
6. The administrator reviews and manages claims, according to the implemented permissions.
7. Users can follow the status of their claims if that functionality is enabled.

---

## Screenshots

Add screenshots of your actual application here after running it successfully.

```markdown
![Home Page](screenshots/home.png)
![Login Page](screenshots/login.png)
![Report Item Page](screenshots/report-item.png)
![Admin Dashboard](screenshots/admin-dashboard.png)
```

Create a `screenshots` directory in the repository and place your screenshot files inside it.

---

## Future Enhancements

- Email notifications for claim updates.
- Image uploads for lost and found items.
- Advanced search and category filters.
- Improved admin analytics and reporting.
- Deployment to a cloud hosting platform.
- Additional security and authorization improvements.

*These are potential enhancements and are not necessarily implemented in the current version.*

---

## Contributing

Contributions and suggestions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Make your changes.
4. Test the application.
5. Submit a pull request.

---

## Author

<div align="center">

  <h3>ArunkumarValandas</h3>

  Full-Stack Java Developer

  <br/><br/>

  <a href="https://github.com/ArunkumarValandas">
    <img src="https://img.shields.io/badge/GitHub-ArunkumarValandas-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub Profile"/>
  </a>

</div>

---

## License

No license has been specified yet. Add a `LICENSE` file if you want to publish this project under a particular open-source license.

---

<div align="center">

  **Built to make campus lost-and-found management easier.**

  <img width="100%" src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=120&section=footer&animation=twinkling" alt="Footer"/>

</div>
