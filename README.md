# ParkEngine – Scalable Parking Allocation System

**Java | Object-Oriented Programming | System Design | Low-Level Design (LLD) | Design Patterns**

## Overview

ParkEngine is a Java-based parking management application that simulates a multi-floor parking facility. It manages vehicle parking, compatible parking-spot allocation, ticket generation, vehicle lookup, parking fee calculation, and vehicle exit operations.

The project demonstrates how object-oriented programming and design patterns can be used to organize a real-world problem into separate classes with clear responsibilities.

## Features

- **Multi-Floor Parking:** Manage parking floors and their parking spots.
- **Multiple Vehicle Types:** Support bikes, cars, and trucks.
- **Parking Spot Allocation:** Select an available spot compatible with the vehicle.
- **Ticket Management:** Generate and track active parking tickets.
- **Vehicle Search:** Find active parking records using a vehicle registration number.
- **Parking Fee Calculation:** Calculate parking charges based on parking duration and the configured pricing strategy.
- **Flexible Pricing:** Demonstrate normal and weekend pricing strategies.
- **Payment Simulation:** Demonstrate Cash, UPI, and Card payment options.
- **Availability Updates:** Notify parking display boards when spot availability changes.
- **Duplicate Entry Prevention:** Prevent duplicate active parking for the same vehicle number.

## Technology Stack

- **Language:** Java
- **Programming Concepts:** OOP, abstraction, inheritance, encapsulation, polymorphism
- **Collections:** ArrayList, HashMap, List, Map
- **Date and Time:** Java Date and Time API
- **Interface:** Console-based menu
- **Version Control:** Git and GitHub

## Design Patterns

| Design Pattern | Purpose |
|---|---|
| Singleton | Maintains a centralized parking-lot instance |
| Factory | Creates vehicle objects based on vehicle type |
| Strategy | Supports interchangeable parking allocation, pricing, and payment behaviours |
| Observer | Notifies display boards when parking availability changes |

These patterns help separate responsibilities and make the application easier to understand and extend.

## Application Workflow

1. A vehicle arrives at the parking facility.
2. The system identifies the vehicle type and registration number.
3. It checks for an existing active parking record.
4. A compatible available parking spot is selected.
5. The vehicle is allocated a spot and a parking ticket is generated.
6. The system tracks the active parking session.
7. At exit, parking duration and applicable charges are calculated.
8. A simulated payment method is invoked.
9. The parking spot is released and availability is updated.

## Project Structure

```text
ParkEngine/
├── src/
│   └── ParkEngine.java
├── README.md
├── .gitignore
└── LICENSE
```

## Prerequisites

- Java Development Kit (JDK)
- A terminal or Java-compatible IDE

## How to Run

Clone the repository:

```bash
git clone https://github.com/Yashec21/ParkEngine-Scalable-Parking-Allocation-System.git
cd ParkEngine-Scalable-Parking-Allocation-System
```

Compile the Java source:

```bash
javac -d out src/ParkEngine.java
```

Run the application:

```bash
java -cp out program1017
```

**Note:** These commands assume the main class is still named `program1017`, as in the current source. If you rename the main class, update the run command accordingly.

## Key Learning Outcomes

- Applying OOP principles to a practical problem.
- Identifying classes, responsibilities, and relationships.
- Using interfaces and abstract classes to define behaviour.
- Applying Singleton, Factory, Strategy, and Observer patterns.
- Managing active records using Java Collections.
- Understanding low-level system design and extensibility.

## Future Enhancements

- Refactor classes into separate packages.
- Add automated unit tests using JUnit.
- Integrate a relational database for persistent storage.
- Develop REST APIs using Spring Boot.
- Improve validation and exception handling.
- Add concurrency-safe parking allocation.
- Develop a graphical or web interface.

## Author

**Yash Patil**

- GitHub: [Yashec21](https://github.com/Yashec21)
- LinkedIn: [yashpatilec](https://www.linkedin.com/in/yashpatilec/)

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.
