# Web-Development-Project

## Overview
**College Shiksha** is a web-based college prediction system that helps students determine which colleges they are eligible to apply for based on their academic scores. The system features user authentication and a smart college predictor algorithm.

## What This Project Does
This project is an educational web application that:
- Provides user registration and login functionality
- Evaluates student performance across multiple entrance exams
- Predicts eligible colleges based on academic scores
- Offers information about various educational institutions in India

## Technology Stack
- **Frontend**: HTML5, CSS3, JavaScript (jQuery)
- **Backend**: PHP (Server-side scripting)
- **Database**: MySQL/MariaDB
- **Server**: Apache (XAMPP)
- **Frameworks/Libraries**: 
  - Bootstrap 4.3.1 (UI styling)
  - Font Awesome 4.7.0 (Icons)
  - jQuery 3.3.1

## Key Features

### 1. User Authentication System
- **Login Page**: Secure user login with username and password
- **Registration**: New user signup functionality
- **Session Management**: PHP sessions to maintain user state
- **Social Media Integration**: Placeholder links for social media platforms

### 2. College Prediction Algorithm
The system predicts college eligibility based on:
- **Board Percentage**: 12th grade marks (minimum 60% required)
- **JEE Score**: Joint Entrance Examination (out of 360)
- **BITS Score**: Birla Institute of Technology and Science entrance exam
- **SRMJEEE Score**: SRM Joint Engineering Entrance Examination
- **VITEEE Score**: VIT Engineering Entrance Examination

### 3. College Recommendations
Based on scores, the system recommends:
- **IIT (Indian Institute of Technology)**: Average > 87%
- **NIT (National Institute of Technology)**: Average > 60%
- **BITS**: Score > 280
- **SRM**: Score > 140
- **VIT**: Score > 80

### 4. About Us Page
Provides detailed information about CollegeShiksha and its services.

## Project Structure
```
Web-Development-Project/
├── login.php           # User login and registration page
├── home.php            # Main college predictor interface
├── practice.php        # About Us page
├── Login.css           # Styling for login page
├── Login.js            # JavaScript for login interactions
├── Home.css            # Styling for home page
├── practice.css        # Styling for about page
├── usertable.sql       # Database schema and sample data
├── jagran_logo1.jpg    # Logo image
├── ScreenShots/        # Application screenshots
│   ├── is1.JPG
│   ├── is2.JPG
│   ├── is3.JPG
│   ├── is4.JPG
│   └── is5.JPG
└── README.md           # Project documentation
```

## Database Schema
**Table**: `usertable`
- `Id` (INT, Primary Key, Auto Increment)
- `Username` (VARCHAR(100))
- `Password` (VARCHAR(100))

## Setup Instructions

### Prerequisites
- XAMPP (Apache + MySQL + PHP)
- Web browser (Chrome, Firefox, etc.)

### Installation Steps
1. Install XAMPP from [https://www.apachefriends.org/](https://www.apachefriends.org/)
2. Clone or download this repository
3. Place the project folder in `C:\xampp\htdocs\` (Windows) or `/opt/lampp/htdocs/` (Linux)
4. Start Apache and MySQL from XAMPP Control Panel
5. Open phpMyAdmin at `http://localhost/phpmyadmin`
6. Create a database named `test_db`
7. Import `usertable.sql` file into the `test_db` database
8. Update the project path in `login.php` (line 55) to match your folder name
9. Access the application at `http://localhost/[your-folder-name]/login.php` (e.g., `http://localhost/Web-Development-Project/login.php`)

## Usage
1. **First-time Users**: Click "Sign Up here" to create an account
2. **Existing Users**: Enter username and password to login
3. **College Prediction**: 
   - Enter your Board percentage (12th grade)
   - Enter scores for various entrance exams (JEE, BITS, SRM, VIT)
   - Click "SUBMIT" to get college recommendations
4. **View Results**: The system displays which colleges you're eligible to apply for

## Security Note
⚠️ **Important**: This project is for educational purposes. In production:
- Passwords should be hashed (use `password_hash()` and `password_verify()`)
- Use prepared statements to prevent SQL injection
- Implement HTTPS for secure data transmission
- Add input validation and sanitization
- Implement CSRF protection

## Screenshots
Screenshots of the application can be found in the `ScreenShots/` directory.

## Contributors
- Indunil Nimesha Jayasooriya

## License
This project is for educational purposes. 
