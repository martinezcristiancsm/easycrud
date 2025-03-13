# Guide to Run the Java Spring Boot Application

OPTION 1:
The project includes an installation script that automates the setup.
Option 1: Run the script automatically

Open a terminal (Git Bash on Windows, Terminal on macOS/Linux).
Run the following command to download and execute the script:

    curl -sSL https://raw.githubusercontent.com/martinezcristiancsm/easycrud/main/install.sh | bash
    
Check the application's port, username and password configured in src/main/resources/application.properties

    spring.datasource.url=jdbc:mysql://localhost:{port_to_use}/easycrud
    spring.datasource.username={username}
    spring.datasource.password={password}
    
This command downloads and runs the script in one step.

If you prefer to download it first and execute it manually, follow 
OPTION2:

## Requirements

- **Java 17 or higher**: Verify with `java -version`.
- **Maven**: Verify with `mvn -v`.

Clone the Repository:

    git clone https://github.com/martinezcristiancsm/easycrud

Navigate to the project directory:

    cd path/to/easycrud

OR

If you already have the repository cloned then navigate to the project directory:

    cd path/to/easycrud

Pull the ultimate changes:

    git pull

Configure the Port, Username, and DB Password

The application's port, username and password is configured in src/main/resources/application.properties. Change the following values to your preferred settings:

    spring.datasource.url=jdbc:mysql://localhost:{port_to_use}/easycrud
    spring.datasource.username={username}
    spring.datasource.password={password}

Build and Run the Application
Build the application:

    mvn clean install

Run the application:

    mvn spring-boot:run

Access the application at http://localhost:8080 (or the port you configured).
