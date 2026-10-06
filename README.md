# Bus Reservation System

Simple Bus Reservation System built with Java 21 + Spring Boot 3.5.6.

## Features
- Search buses by source and destination
- View bus schedules and prices
- Interactive seat selection
- Passenger details and reservation confirmation
- Booking ID generation
- View current bookings
- Cancel bookings
- No database required; data is stored in memory
- Responsive web UI
- Docker support

## Requirements
- Java 21
- Maven 3.9+ (or use Docker without installing Maven)

## Run locally on Windows PowerShell

```powershell
cd bus-reservation-system
mvn clean package
java -jar targetus-reservation-system-1.0.0.jar
```

Open:
http://localhost:8080

If Maven is not installed but Java is installed, use Docker instead.

## Run with Docker

```powershell
cd bus-reservation-system
docker build -t bus-reservation-system .
docker run --name bus-reservation-system -p 8080:8080 bus-reservation-system
```

Open:
http://localhost:8080

Stop:
```powershell
docker stop bus-reservation-system
```

Remove:
```powershell
docker rm bus-reservation-system
```

## Run with Docker Compose

```powershell
cd bus-reservation-system
docker compose up --build
```

Open:
http://localhost:8080

Stop:
```powershell
docker compose down
```

## Important
There is intentionally no database. Restarting the application clears bookings and restores the sample bus data.
