# Employee Time Tracker

A modern, responsive web application for visualizing employee time data through interactive tables and charts. This application fetches time entries from an API endpoint and displays comprehensive analytics about employee working hours.

##  Features

### Core Functionality
- *Employee Table*: Sortable table displaying employees ordered by total time worked
- *Visual Indicators*: Rows highlighted in red for employees with less than 100 hours
- *Interactive Pie Chart*: Visual distribution of time worked by each employee
- *Real-time Statistics*: Cards showing total employees, total hours, and low-hour count
- *Dual Data Sources*: Toggle between real API data and mock data

### Technical Features
- *Responsive Design*: Works seamlessly on desktop, tablet, and mobile devices
- *CORS Handling*: Graceful error handling with automatic fallback to mock data
- *Modern UI*: Gradient backgrounds, smooth animations, and professional styling
- *Chart Interactions*: Hover effects, tooltips showing hours and percentages
- *Performance Optimized*: Efficient data processing and rendering

##  Data Visualization

### Employee Performance Categories
- *🟢 High Performers (100+ hours)*: Regular background color
- *🔴 Needs Attention (<100 hours)*: Highlighted in red/pink with left border accent

### Analytics Dashboard
- *Total Employees Count*: Real-time count of all employees
- *Total Hours Worked*: Sum of all employee hours across the organization
- *Low Hours Alert*: Count of employees requiring attention (<100 hours)

##  Technical Implementation

### Architecture
- *Frontend*: Pure JavaScript (no framework dependencies for maximum compatibility)
- *Charts*: Chart.js 4.4.0 for interactive data visualization
- *Styling*: Modern CSS with flexbox and grid layouts
- *Data Processing*: Client-side aggregation and sorting of time entries

### API Integration
```javascript
// API Endpoint
const apiUrl = 'https://rc-vault-fap-live-1.azurewebsites.net/api/gettimeentries?code=vO17RnE8vuzXzPJo5eaLLjXjmRW07law99QTD90zat9FfOQJKKUcgQ=='

// Data Structure Expected
{
  "EmployeeName": "string",
  "StarTimeUtc": "2022-02-01T08:00:00",
  "EndTimeUtc": "2022-02-01T17:00:00",
  "EntryNotes": "string",
  "DeletedOn": null
}
