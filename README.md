# ParkEngine – Scalable Parking Allocation System

ParkEngine is a Java-based parking management application that simulates vehicle parking across multiple floors. It manages parking spot allocation, ticket generation, vehicle lookup, parking fee calculation, and exit processing.

The project demonstrates object-oriented programming, low-level design, and commonly used design patterns through a modular parking system.

## Features

- **Multi-Floor Parking:** Manage parking floors with dedicated spots for bikes, cars, and trucks.
- **Automated Spot Allocation:** Allocate the first available compatible parking spot.
- **Ticket Management:** Generate parking tickets and track active parking sessions.
- **Vehicle Search:** Find an active parking ticket using the vehicle number.
- **Parking Fee Calculation:** Calculate charges based on vehicle type and parking duration.
- **Flexible Pricing:** Support normal and weekend pricing strategies.
- **Payment Simulation:** Demonstrate Cash, UPI, and Card payment options.
- **Availability Updates:** Refresh parking display boards when spot availability changes.
- **Duplicate Entry Prevention:** Prevent the same vehicle from being parked more than once during an active session.

## Tech Stack

- **Language:** Java
- **Core Concepts:** OOP, Collections Framework, Exception Handling, Java Date and Time API
- **Data Structures:** ArrayList, HashMap, List, Map
- **Design Patterns:** Singleton, Factory, Strategy, Observer
- **Interface:** Console-based menu

## Design Patterns

| Pattern | Implementation | Purpose |
|---|---|---|
| Singleton | `ParkingLot` | Provides a shared parking lot instance |
| Factory | `VehicleFactory` | Centralizes vehicle object creation |
| Strategy | `ParkingStrategy` | Separates parking spot selection logic |
| Strategy | `PricingStrategy` | Separates parking fee calculation |
| Strategy | `PaymentStraregy` | Supports interchangeable payment implementations |
| Observer | `ParkingObserver` | Updates display boards when parking availability changes |

## How It Works

1. Select the vehicle type and enter its registration number.
2. The system checks for duplicate active parking.
3. An available compatible parking spot is selected.
4. The entry gate generates a parking ticket.
5. At exit, the system calculates parking duration and charges.
6. A payment method is selected and the parking spot is released.

## Project Structure

```text
ParkEngine/
├── src/
│   └── program1017.java
├── screenshots/
├── README.md
├── .gitignore
└── LICENSE
```

The current implementation keeps the application classes in a single Java source file. The project can be further modularized into separate packages.

## Prerequisites

- Java Development Kit (JDK) installed
- A terminal or Java-compatible IDE
- Git (optional, for cloning and version control)

## How to Run

Clone the repository:

```bash
git clone https://github.com/Yashec21/ParkEngine.git
cd ParkEngine
```

Compile the application from the repository root:

```bash
javac -d out src/program1017.java
```

Run the application:

```bash
java -cp out program1017
```

The application presents a console menu for parking vehicles, processing exits, searching vehicles, and displaying parking information.

## Learning Outcomes

- Applying OOP principles to a real-world use case
- Designing interchangeable algorithms using Strategy Pattern
- Centralizing object creation with Factory Pattern
- Implementing event-driven updates with Observer Pattern
- Managing application state using Java Collections
- Modeling parking sessions with Java Date and Time API

## Future Scope

- Refactor classes into separate Java packages
- Add automated unit tests using JUnit
- Persist parking records using MySQL or PostgreSQL
- Develop REST APIs using Spring Boot
- Add concurrency-safe parking allocation
- Integrate a graphical interface and real payment gateway

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Author

**Yash Patil**

- GitHub: [Yashec21](https://github.com/Yashec21)
- LinkedIn: [yashpatilec](https://www.linkedin.com/in/yashpatilec/)
