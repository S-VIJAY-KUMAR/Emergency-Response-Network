# Emergency Response Network (ERN)

## Team Details
- **Team ID:** LTVIP2025TMID27092
- **Team Leader:** S. Vijay Kumar
- **Team Members:**
  - C. Prathibha
  - K. Siddesh
  - P. Sudarshan
  - V. Vamshi

---

## Project Overview
The **Emergency Response Network (ERN)** is a backend system designed to streamline emergency response operations. Built with **Node.js**, **Express.js**, and **MongoDB**, ERN handles emergency request registrations, assigns responders, and provides real-time updates to authorities and volunteers.

### Key Features:
- **Emergency Request Registration:** Users can report emergencies via API.
- **Automated Responder Assignment:** Based on proximity and availability.
- **Real-Time Updates:** Responder locations and incident status updates.
- **User Authentication:** Secure access for users, volunteers, and admins.
- **Incident Logging & Reporting:** Historical data for future analysis.

---

## Scenario-Based Case Study
**Scenario: Fire Emergency in a Residential Area**
1. Resident reports a fire via a mobile app.
2. Backend logs the request and identifies nearby fire stations.
3. Responders receive location-based alerts.
4. Authorities monitor incident progress in real time.

---

## Technical Architecture
The system is based on a **Microservices REST API architecture**.
- **Backend:** Node.js, Express.js
- **Database:** MongoDB (Mongoose ODM)
- **Authentication:** JWT (JSON Web Tokens)
- **API Testing:** Postman / Thunderclient

---

## Database Design
- **Users Collection:** Stores details of users, responders, and admins.
- **Emergencies Collection:** Stores reported incidents.
- **Reports Collection:** Logs incident details for analysis.

---

## API Endpoints (Demo Focus)

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

### Report Routes
- **Create Report:** `POST /report/create`
- **Get All Reports:** `GET /report/all`
- **Get Nearby Reports:** `GET /report/near/:location`
- **Filter Reports:** `GET /report/filter?<query>`

### Alerts
- **Get Alerts:** `GET /alert/any`

---

## Project Setup (For Demo)
1. **Install Node.js & MongoDB**
2. **Clone the Repository:** `git clone [repository_url]`
3. **Install Dependencies:** `npm install`
4. **Configure Environment Variables:**
   - `JWT_SECRET`
   - `MONGODB_URI`
5. **Run the Server:** `npm start`

---

## Demo Flow
1. **User Registration & Login:**
   - Register and log in a user via Postman.
2. **Emergency Creation & Alerts:**
   - Simulate an emergency and view responder alerts.
3. **Real-Time Updates:**
   - Show incident status changing via API.
4. **Data Visualization:**
   - Query logs and reports to display historical data.

---

## Conclusion
The **Emergency Response Network** is a powerful, scalable backend solution that enhances emergency response through automation and real-time updates. It bridges the gap between victims, volunteers, and authorities — ensuring swift action during critical situations.


