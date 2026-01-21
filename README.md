# Court 9 Badminton Center Queue Management System

A comprehensive management system for badminton centers with matchmaking, e-commerce, stringing services, reservations, and tournament management.

![Badges](https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white)
![Badges](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Badges](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Badges](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)

## Overview

The Court 9 Badminton Center Queue Management System is a comprehensive web application designed to streamline operations for badminton centers. It integrates multiple functionalities into a single platform to manage player matchmaking, court reservations, e-commerce operations, stringing services, and tournament management.

## Features

### 🏸 Matchmaking Rating
Intelligent player matchmaking based on skill ratings, availability, and preferences. Implements an ELO-like rating system to ensure balanced and competitive matches.

### 🛒 E-Commerce (Point of Sales)
Complete POS system for managing sales of badminton equipment, merchandise, and court bookings. Includes inventory management, sales reports, and payment processing integration.

### 🎾 Stringing Services
Manage racquet stringing requests with service tracking, pricing, and scheduling. Customers can select string types, tension preferences, and track completion status.

### 📅 Reservation System
Interactive court reservation system with real-time availability, automated scheduling, and payment integration. Supports recurring bookings and group reservations.

### 🏆 Club Tournaments System
Organize and manage tournaments with automated bracket generation, participant registration, score tracking, and result publishing. Supports different tournament formats.

## Technology Stack

- **Backend**: Laravel 9+, PHP 8.1+, MySQL
- **Frontend**: Tailwind CSS, JavaScript (ES6+)
- **Tools**: Composer, npm/Yarn, Git

### Prerequisites
- PHP >= 8.1
- Composer
- Node.js & npm
- MySQL >= 5.7

## Installation

```bash
# Clone the repository
git clone https://github.com/ayumihidalgo/E-skolarian.git

# Install PHP dependencies
composer install 

# Install NPM dependencies
npm install

# Create a copy of your .env file
cp .env.example .env

# Generate an app encryption key
php artisan key:generate

# Configure your database in .env (or you can copy this)
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=court9remastered
DB_USERNAME=root
DB_PASSWORD=

# Run database migrations
php artisan migrate

# Compile assets
npm run dev

# Run server
php artisan serve
```

2. Update the php.ini File
Locate the php.ini file used by your PHP installation. You can find it by running the following command in your terminal:

``` bash 
php --ini
```
Open the php.ini file in a text editor. 

Remove the semicolon of the following:
- ;extension=zip
- ;extension=mbstring
- ;extension=fileinfo
- ;extension=curl

3. Restart Your Web Server using 
```bash
php artisan serve
```

## Usage

<details>
<summary>Click to expand usage instructions</summary>

1. Start the Laravel development server:
   ```
   php artisan serve
   ```
2. Start the compile of assets:
  ```
  npm run dev
  ```
3. Access the web interface at `http://localhost:8000`
4. Make sure apache and mysql is running when you are using XAMPP
5. Keep both 1 and 2 running on terminal during development

