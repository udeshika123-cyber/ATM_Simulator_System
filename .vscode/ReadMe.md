# ATM Simulator System

This is a Java-based ATM Simulator System project. It provides a graphical user interface for simulating ATM operations such as account signup, login, balance enquiry, deposit, withdrawal, and more.

## Project Structure

```
ATM-Simulator-System/
├── build.xml
├── manifest.mf
├── .vscode/
│   └── launch.json
├── build/
│   └── classes/
├── lib/
│   ├── jcalendar-tz-1.3.3-4.jar
│   └── mysql-connector-java-8.0.28.jar
├── nbproject/
│   ├── build-impl.xml
│   ├── genfiles.properties
│   ├── project.properties
│   ├── project.xml
│   └── private/
├── src/
│   └── ASimulatorSystem/
│       ├── BalanceEnquiry.class
│       ├── BalanceEquiry.java
│       ├── Conn.class
│       ├── Conn.java
│       ├── Deposit.class
│       ├── Deposit.java
│       ├── FastCash.class
│       ├── FastCash.java
│       └── ...
```

## Getting Started

### Prerequisites

- Java JDK 8 or higher
- [Apache Ant](https://ant.apache.org/) (for building)
- MySQL (for backend database)
- The following libraries (already included in `lib/`):
  - jcalendar-tz-1.3.3-4.jar
  - mysql-connector-java-8.0.28.jar

### Building the Project

To build the project, run:

```sh
ant clean
ant build
```

Or use your IDE's build functionality.

### Running the Project

You can run the project using the provided VS Code launch configuration or by running the main class:

```sh
ant run
```

Or, if running manually:

```sh
java -cp "build/classes;lib/*" ASimulatorSystem.Login
```

### Main Classes

- [`ASimulatorSystem.Login`](src/ASimulatorSystem/Login.java) - Main entry point for the ATM login screen.
- [`ASimulatorSystem.Signup`](src/ASimulatorSystem/Signup.java) - Handles new account signups.
- [`ASimulatorSystem.Signup2`](src/ASimulatorSystem/Signup2.java) - Additional details for signup.
- [`ASimulatorSystem.Signup3`](src/ASimulatorSystem/Signup3.java) - Account details and confirmation.
- [`ASimulatorSystem.BalanceEnquiry`](src/ASimulatorSystem/BalanceEnquiry.java) - Balance enquiry functionality.
- [`ASimulatorSystem.Deposit`](src/ASimulatorSystem/Deposit.java) - Deposit functionality.
- [`ASimulatorSystem.FastCash`](src/ASimulatorSystem/FastCash.java) - Fast cash withdrawal.

## Configuration

- Database connection settings are managed in [`ASimulatorSystem.Conn.java`](src/ASimulatorSystem/Conn.java).
- Libraries are located in the `lib/` directory.

## License

This project is for educational purposes.