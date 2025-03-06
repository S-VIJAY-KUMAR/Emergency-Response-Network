# Emergency Response Network

## Project Details

- **Project Name:** Emergency Response Network
- **Team ID:** LTVIP2025TMID27092
- **Team Leader:** S. Vijay Kumar
- **Team Members:**
  - C. Prathibha
  - K. Siddesh
  - P. Sudarshan
  - V. Vamshi

## Project Overview

The Emergency Response Network (ERN) is a robust system designed to streamline emergency management. It registers emergency requests, alerts responders, and provides real-time updates. Built with Node.js, Express.js, and MongoDB, the backend supports seamless integration with mobile apps, web dashboards, and IoT devices.

### Key Functionalities:

- **Emergency Request Registration:** Users can report emergencies via API.
- **Real-time Alerts:** Notifies responders immediately.
- **Automated Responder Assignment:** Based on proximity and availability.
- **Incident Status Updates:** Tracks and logs incidents.

## Scenario-Based Case Study

**Scenario:** Fire Emergency in a Residential Area

1. A resident reports a fire via the mobile app.
2. The backend logs the request into MongoDB.
3. Nearby fire stations and available trucks are identified.
4. Responders receive notifications with live location tracking.
5. Authorities monitor incident updates in real-time.

This case study illustrates ERN’s capacity to streamline emergency responses through automated, data-driven processes.

## Technical Architecture

The system follows a Microservices-based REST API architecture, ensuring modularity and scalability.

### Technology Stack:

- **Backend:** Node.js, Express.js
- **Database:** MongoDB (Mongoose ODM)
- **Authentication:** JWT-based authentication
- **API Testing:** Postman / Thunderclient

## ER Diagram

The database structure includes the following entities:

- **Users:** Stores users, victims, volunteers, and admin details.
- **Emergencies:** Stores reported emergencies.
- **Reports:** Logs incident history for analysis.

## Key Features

- **Automated Emergency Response:** Alerts responders based on proximity.
- **Real-time Updates:** Tracks responders and incidents.
- **User Authentication & Role Management:** Secure access control.
- **Incident Logging & Reports:** Maintains historical records.
- **Multi-Platform API Integration:** Supports mobile, web, and IoT apps.

## Prerequisites

Before setting up the project, ensure you have:

- **Node.js (Latest LTS version)** installed
- **MongoDB Database Setup** (Local or Cloud-based, e.g., MongoDB Atlas)
- **Postman** or **Thunderclient** for API testing
- **Code Editor:** VS Code or any preferred IDE
- **Basic Knowledge:** JavaScript, Node.js, and MongoDB

## Roles & Responsibilities

### 1. Users (Emergency Reporters)

- Register and log in.
- Report emergencies with location and incident details.

### 2. Volunteers (Responders)

- Register and verify as responders.
- Receive alerts based on location and availability.

### 3. Admins (System Managers)

- Manage users and volunteers.
- Oversee emergency reports and responses.

## Application Flow

1. Users send emergency requests via API.
2. The system validates and logs the incident.
3. Volunteers are alerted and track incidents in real-time.
4. Authorities monitor ongoing incidents.

## Project Setup & Configuration

- Initialize the project with Node.js and Express.js.
- Configure **package.json** and install dependencies:
  ```bash
  npm install express mongoose dotenv jsonwebtoken cookie-parser bcrypt
  ```
- Set up environment variables (e.g., `JWT_SECRET`, `MONGODB_URI`).

## Backend Development

- Create RESTful APIs for emergency handling, authentication, and incident updates.
- Implement JWT-based authentication.
- Define controllers and middleware for request handling.

## Database Design

- Design MongoDB schemas:
  - **Users:** Stores user data.
  - **Emergencies:** Stores reported emergencies.
  - **Reports:** Stores historical incidents.
- Use MongoDB Compass or Atlas for visualization.

## API Testing

Use **Postman** or **Thunderclient** to test API endpoints:

### User Routes

- **Register:** `POST /user/register`
- **Login:** `POST /user/login`
- **Update Profile:** `POST /user/update`
- **Logout:** `POST /user/logout`

### Emergency Routes

- **Create Emergency:** `POST /emergency/create`
- **Update Emergency:** `PUT /emergency/update`
- **Get All Emergencies:** `GET /emergency/all`
- **Get Nearby Emergencies:** `GET /emergency/near/:location`
- **Filter Emergencies:** `GET /emergency/filter?<query>`

### Report Routes

- **Create Report:** `POST /report/create`
- **Get All Reports:** `GET /report/all`
- **Get Nearby Reports:** `GET /report/near/:location`
- **Filter Reports:** `GET /report/filter?<query>`

## Outputs (API Testing)

Example responses:

- **Unauthorized Request:** 401 status for unauthenticated access.
- **Successful Report Creation:** 201 status with report ID.
- **Responder Alert:** Real-time alert with incident details.

## Conclusion

The Emergency Response Network (ERN) is a powerful, scalable, and life-saving system designed to revolutionize emergency management. By integrating real-time data handling, proximity-based responder assignment, and multi-platform support, ERN ensures faster, more efficient, and data-driven emergency responses.

---

🔧 **Developed by Team LTVIP2025TMID27092** 🚀

If you have any questions or need assistance, feel free to reach out to the team leader, **S. Vijay Kumar**.



