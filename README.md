<div align="center">

# 🐠 Prestige Koi Auction

### A Modern Platform for Premium Koi Fish Auctions

[Features](#features) • [Installation](#installation) • [Usage](#usage) • [Documentation](#documentation) • [Support](#support)

![Build Status](https://img.shields.io/badge/build-passing-brightgreen)
![Version](https://img.shields.io/badge/version-1.0.0-blue)
![License](https://img.shields.io/badge/license-MIT-green)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=oracle&logoColor=white)

</div>

---

## 🎯 Overview

Prestige Koi Auction is a sophisticated digital marketplace designed specifically for the premium koi fish auction industry. Our platform bridges the gap between koi breeders and enthusiasts, offering a transparent, secure, and efficient auction experience.

### 🎭 Key Roles

- **Koi Breeders**: Showcase and sell premium koi
- **Managers**: Oversee auction operations
- **Staff**: Handle inspections and verifications
- **Members**: Participate in auctions
- **Guests**: Browse available lots

## ✨ Features

### 🔐 Security & Authentication
- JWT-based secure authentication
- Role-based access control
- Protected transaction handling

### 🏷️ Auction Management
- **Multiple Auction Types**
  - Fixed Price Sales
  - Sealed Bids
  - Ascending Auctions
  - Descending Auctions
- Real-time bidding system
- Automated slot management

### 💎 Premium Features
- **Quality Assurance**
  - Professional fish inspection
  - Detailed documentation
  - Verification process
- **Financial Management**
  - Secure deposit system
  - Automated refunds
  - Transparent fee structure

## 🛠️ Tech Stack

<div align="center">

| Layer | Technologies |
|-------|--------------|
| Frontend | ![React](https://img.shields.io/badge/React-20232A?style=flat&logo=react&logoColor=61DAFB) ![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat&logo=vite&logoColor=white) ![Tailwind](https://img.shields.io/badge/Tailwind-38B2AC?style=flat&logo=tailwind-css&logoColor=white) |
| Backend | ![Java](https://img.shields.io/badge/Java-ED8B00?style=flat&logo=java&logoColor=white) ![Spring](https://img.shields.io/badge/Spring-6DB33F?style=flat&logo=spring&logoColor=white) |
| Database | ![MSSQL](https://img.shields.io/badge/MSSQL-CC2927?style=flat&logo=microsoft-sql-server&logoColor=white) |
| DevOps | ![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat&logo=docker&logoColor=white) ![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat&logo=amazon-aws&logoColor=white) |

</div>

## 🚀 Installation

### Prerequisites

```bash
Java 21
Node.js 18+
MSSQL 2019+
Maven 3.9+
Redis Server
```

### Database Setup

1. Create the database:
```sql
CREATE DATABASE Koi_project
```

2. Configure connection in `application.properties`:
```properties
spring.datasource.url=jdbc:sqlserver://localhost:1433;databaseName=Koi_project;encrypt=true;trustServerCertificate=true
spring.datasource.username=sa
spring.datasource.password=Password@123
```

3. Initialize core data:
```sql
INSERT INTO AuctionType(auctionTypeName) VALUES
('FIXED_PRICE_SALE'),
('SEALED_BID'),
('ASCENDING_BID'),
('DESCENDING_BID');

INSERT INTO Variety(varietyName) VALUES
('Kohaku'),
('Taisho Sanke'),
('Showa'),
('Shiro Utsuri'),
('Utsurimono'),
('Beni Kikokuryu'),
('Asagi'),
('Kikokuryu'),
('Hikari Muji'),
('Goshiki');
```

### Backend Setup

1. Start Redis server
2. Launch the Spring Boot application
3. Create initial manager account:
```bash
GET http://localhost:8080/authenticate/create-manager-account
```

### Frontend Setup

```bash
npm install
npm run dev
```

## 📚 Documentation

### Project Structure
```
prestige-koi-auction/
├── backend/
│   ├── src/
│   └── pom.xml
├── frontend/
│   ├── src/
│   └── package.json
└── README.md
```

### Default Credentials
```
Manager Account:
Email: manager@gmail.com
Password: @manager1

VNPay Test Card:
Card Number: 9704195798459170488
Name: NGUYEN VAN A
Issue Date: 07/15
OTP: 123456
```


## 🤝 Support

Need help? We're here for you!

- 📫 Email: [mentionable9999@gmail.com](mailto:mentionable9999@gmail.com)

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.

---

<div align="center">

Made with ❤️ by the Prestige Koi Auction Team

</div>
