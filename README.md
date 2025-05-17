# ReactCustomAuth

A custom React user registration form with client-side validation, visual feedback, and JSON Server as a mock backend API.

![React](https://img.shields.io/badge/React-18.2.0-blue)
![JSON Server](https://img.shields.io/badge/JSON_Server-v0.17.1-green)
![Axios](https://img.shields.io/badge/Axios-v1.4.0-orange)

---

## Table of Contents

- [About](#about)  
- [Features](#features)  
- [Tech Stack](#tech-stack)  
- [Installation](#installation)  
- [Usage](#usage)  
- [API Details](#api-details)  
- [Validation Rules](#validation-rules)  
- [Contributing](#contributing)  
- [License](#license)

---

## About

**ReactCustomAuth** is a React-based user registration form that validates inputs in real-time using regular expressions and provides instant visual feedback using FontAwesome icons. It uses Axios to interact with a mock backend powered by JSON Server, enabling easy prototyping of registration workflows without needing a full backend.

---

## Features

- Real-time validation for username and password fields  
- Password confirmation matching  
- Error handling with descriptive messages  
- Visual validation feedback using icons  
- Data submission to a JSON Server mock REST API  
- Accessible and responsive form design

---

## Tech Stack

- React (Functional Components with Hooks)  
- Axios for HTTP requests  
- JSON Server as a mock REST API  
- FontAwesome for icons  
- Custom CSS for styling and feedback

---

## Installation

1. **Clone the repo**  
   ```bash
   git clone https://github.com/your-username/reactcustomauth.git
   cd reactcustomauth
Install dependencies

bash
Copy code
npm install
Install JSON Server globally (if you haven't yet)

bash
Copy code
npm install -g json-server
Start JSON Server

bash
Copy code
json-server --watch src/data/db.json --port 3500
Run the React app

bash
Copy code
npm start
Usage
Navigate to http://localhost:3000 in your browser

Complete the registration form

Submit to send the data to JSON Server backend at http://localhost:3500/users

On success, a confirmation message will appear

API Details
Base URL: http://localhost:3500

Endpoint: /users

The JSON Server watches src/data/db.json for storing registered users

Example structure inside db.json:

json
Copy code
{
  "users": [
    {
      "id": 1,
      "username": "exampleUser",
      "password": "ExamplePass123!"
    }
  ]
}
Validation Rules
Username

4 to 24 characters

Must start with a letter

Allowed characters: letters, numbers, underscores, hyphens

Password

8 to 24 characters

Must contain uppercase and lowercase letters

Must include a number

Must include one special character (! @ # $ %)

Confirm Password

Must exactly match the password field

Contributing
Contributions are welcome! Please open issues or submit pull requests to improve this project.
