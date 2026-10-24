# 🗑️ Garbage Collector

A web-based waste management platform that connects citizens, garbage collectors, and administrators to make waste reporting and collection more efficient.

## 🚀 Features

- **Citizen Dashboard:** Report garbage and track report status.
- **Photo Evidence:** Capture waste photos using the device camera.
- **GPS Location:** Record the location where waste is reported.
- **Collector Dashboard:** View reports and manage cleaning tasks.
- **Navigation:** Open Google Maps directions to the reported location.
- **Report Management:** Track reports as Open, In Progress, or Resolved.
- **Admin Dashboard:** Monitor reports, users, and service areas.
- **Priority System:** Prioritize reports based on severity, age, and nearby unresolved reports.
- **Notifications:** Inform users about report updates.
- **Database:** Store user accounts and reports for future access.
- **Phone Number Validation:** Prevent duplicate account registration using the same phone number.

## 🛠️ Technologies Used

- HTML5
- CSS3
- JavaScript
- Node.js and Express.js (backend, if configured)
- SQLite (database, if configured)
- Browser Geolocation API
- Camera API
- Google Maps Directions

## 📂 Project Modules

### 1. Citizen
- Register and log in.
- Submit garbage reports with photos and GPS coordinates.
- Select garbage category and severity.
- View previously submitted reports.
- Track report resolution.

### 2. Garbage Collector
- View assigned reports and priorities.
- Navigate to garbage locations using Google Maps.
- Start cleaning tasks.
- Upload after-cleaning photos.
- Mark completed reports as resolved.

### 3. Administrator
- Monitor all reports.
- Manage users and service areas.
- Assign collectors to service areas.
- Track report statuses and overall activity.

## ⚙️ Installation and Setup

### Prerequisites
- Node.js and npm, if using the backend version.
- Visual Studio Code.
- A modern web browser.

### Run the Project

1. Download or clone the repository.
2. Open the project folder in VS Code.
3. Open the integrated terminal.
4. Install dependencies if a `package.json` file is present:

   ```bash
   npm install
   ```

5. Start the backend if an `npm start` script is configured:

   ```bash
   npm start
   ```

6. Open the local URL printed by the server. For a server configured on port 3000, use:

   `http://localhost:3000`

**Note:** Follow the actual project configuration if its scripts or port differ.

## 🗺️ Navigation

Collectors can open directions to the GPS coordinates associated with a waste report using Google Maps.

The standard Google Maps Directions URL does not require a Google Maps API key. Advanced embedded maps or routing features may require additional API configuration.

## 🗄️ Database

The intended database functionality includes:

- User account storage.
- Unique phone number validation.
- Waste report history.
- GPS coordinates and report descriptions.
- Collector assignments.
- Report status and timestamps.
- Before-and-after photo references.

A server-side database and backend validation are required for reliable persistence across devices. Browser `localStorage` alone does not provide shared database storage.

## 🔐 Security

- Enforce phone number uniqueness on the server and in the database.
- Use real OTP verification for production.
- Protect administrator and collector operations with authentication and authorization.
- Restrict Google Maps API keys to required APIs and authorized websites.
- Never upload API keys, credentials, or personal data to a public repository.
- Use HTTPS when deploying the application.
- Validate uploaded images and incoming data.

## 🔮 Future Improvements

- Live collector location tracking.
- Estimated arrival time.
- Route optimization for multiple reports.
- Real-time notifications.
- Analytics and waste collection reports.
- Cloud photo storage.
- Mobile-friendly Progressive Web App (PWA).

## 📄 License

No license has been specified yet. Add a license before distributing the project publicly.
