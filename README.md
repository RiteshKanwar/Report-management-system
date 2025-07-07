# Report Management System

A comprehensive web-based report management system built with Google Apps Script that provides secure authentication, equipment tracking, and streamlined report generation capabilities.

## 🚀 Features

- **User Authentication**: Secure login system with session management
- **Report Management**: Create, view, edit, and manage reports efficiently
- **Equipment Tracking**: Monitor and manage equipment-related data
- **Web Interface**: Clean, responsive HTML interface for easy navigation
- **Database Integration**: Seamless data storage and retrieval using Google Sheets
- **Utility Functions**: Comprehensive helper functions for enhanced functionality

## 📁 Project Structure

```
Report Management System/
├── Authentication.gs    # User authentication and session management
├── Code.gs             # Main application entry point and core logic
├── Database.gs         # Database operations and data management
├── Equipment.gs        # Equipment-related functionality and tracking
├── Home.html          # Main dashboard and home page interface
├── Login.html         # User login interface
├── Reports.gs         # Report generation, management, and processing
├── UI.gs              # User interface functions and web app routing
└── Utilities.gs       # Helper functions and utility methods
```

## 🛠️ File Descriptions

### Backend Scripts (.gs files)

- **`Authentication.gs`**: Handles user login, logout, session validation, and security protocols
- **`Code.gs`**: Contains the main application logic and serves as the primary entry point
- **`Database.gs`**: Manages all database operations including CRUD operations with Google Sheets
- **`Equipment.gs`**: Provides equipment management functionality, tracking, and related operations
- **`Reports.gs`**: Handles report creation, modification, data processing, and export features
- **`UI.gs`**: Manages web app routing, HTML serving, and user interface interactions
- **`Utilities.gs`**: Contains helper functions, data validation, formatting utilities, and common operations

### Frontend Files (.html)

- **`Home.html`**: Main dashboard displaying system overview, navigation, and key metrics
- **`Login.html`**: User authentication interface with login form and validation

## 🚀 Setup Instructions

### Prerequisites
- Google Account with access to Google Apps Script
- Google Sheets for database storage
- Basic understanding of Google Apps Script environment

### Installation Steps

1. **Create a new Google Apps Script project**
   ```
   1. Go to script.google.com
   2. Click "New Project"
   3. Give your project a meaningful name
   ```

2. **Upload the script files**
   ```
   1. Copy the content of each .gs file into corresponding script files
   2. Create HTML files for Home.html and Login.html
   3. Ensure all files are properly named as listed above
   ```

3. **Set up Google Sheets database**
   ```
   1. Create a new Google Sheets document
   2. Configure sheets for your data structure
   3. Note the Spreadsheet ID for database configuration
   ```

4. **Configure the application**
   ```
   1. Update database connection settings in Database.gs
   2. Configure authentication parameters in Authentication.gs
   3. Set up any required API keys or permissions
   ```

5. **Deploy the web application**
   ```
   1. Click "Deploy" > "New Deployment"
   2. Choose "Web app" as the type
   3. Set execute permissions and access levels
   4. Deploy and copy the web app URL
   ```

## 💻 Usage

### Accessing the System
1. Navigate to your deployed web app URL
2. Log in using your credentials on the Login page
3. Access the main dashboard through Home.html
4. Navigate through different sections using the interface

### Core Functionalities
- **Report Creation**: Use the reports section to create new reports
- **Equipment Management**: Track and manage equipment through dedicated tools
- **Data Management**: View, edit, and organize your data efficiently
- **User Management**: Handle authentication and user sessions

## 🔧 Configuration

### Database Setup
Update the spreadsheet ID and range configurations in `Database.gs`:
```javascript
const SPREADSHEET_ID = 'your-spreadsheet-id-here';
const REPORTS_SHEET = 'Reports';
const EQUIPMENT_SHEET = 'Equipment';
```

### Authentication Settings
Configure authentication parameters in `Authentication.gs` as needed for your security requirements.

## 📋 API Reference

### Main Functions
- `doGet()`: Handles HTTP GET requests and serves appropriate HTML pages
- `doPost()`: Processes form submissions and POST requests
- `authenticateUser()`: Validates user credentials
- `createReport()`: Generates new reports
- `getEquipmentData()`: Retrieves equipment information
- `updateDatabase()`: Handles database updates

## 🤝 Contributing

1. Fork the project
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🐛 Troubleshooting

### Common Issues
- **Authentication Problems**: Check user permissions and authentication settings
- **Database Errors**: Verify spreadsheet ID and sheet names in Database.gs
- **Deployment Issues**: Ensure proper permissions are set during deployment

### Support
For additional support or questions:
1. Check Google Apps Script documentation
2. Review error logs in the Apps Script editor
3. Verify all required permissions are granted

---

**Built with ❤️ using Google Apps Script**
