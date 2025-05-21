# AFI Machinery Maintenance System

A Google Apps Script web application for managing machinery maintenance at Advanced Food Industries (AFI).

## About

شركة الصناعات الغذائية المتطورة (Advanced Food Industries Company) is a leading food manufacturing enterprise specializing in meat processing, rice packaging, and traditional maamoul production. This maintenance management system streamlines machine maintenance operations across all production departments.

## Overview

This system provides a comprehensive solution for tracking and managing machinery maintenance operations. Built with a mobile-first approach, it ensures optimal performance and usability for technicians working on the production floor. The interface features Arabic language support and is designed to work seamlessly across all devices.

## Screenshots

### Dashboard
![Dashboard View](docs/screenshots/dashboard.png)
*Main dashboard showing machine status and maintenance overview*

### Machine Details
![Machine Details](docs/screenshots/machine-details.png)
*Detailed view of individual machine information and maintenance history*

### Maintenance Schedule
![Maintenance Schedule](docs/screenshots/maintenance-schedule.png)
*Calendar view of scheduled maintenance activities*

### Mobile View
![Mobile Interface](docs/screenshots/mobile-view.png)
*Responsive mobile interface for on-the-go access*

## Key Benefits

- Reduces unplanned downtime by up to 38%
- Extends equipment lifespan through preventive maintenance
- Improves maintenance team efficiency
- Enhances decision-making with detailed equipment history
- Maintains compliance with food safety regulations
- Optimized for mobile use on the production floor

## Features

- Machine management and tracking
- Maintenance scheduling and monitoring
- Real-time status updates (Operational, Maintenance, Breakdown)
- Search and filter functionality
- Mobile-first responsive design
- Touch-optimized interface for field use
- Arabic language support (RTL layout)
- Performance analytics (MTBF, MTTR, uptime)
- Document management for equipment manuals and certificates
- Offline capability for areas with limited connectivity

## Technical Stack

- Google Apps Script
- HTML/CSS/JavaScript
- Google Sheets API (v4)
- Custom AFI Library
- AFI Controller Library (Handles all database CRUD operations)
- Progressive Web App (PWA) features for mobile optimization

## Database Operations

The system uses the AFI Controller library to manage all database operations:
- Create: Adding new machines and maintenance records
- Read: Retrieving machine data and maintenance history
- Update: Modifying machine status and maintenance schedules
- Delete: Removing outdated records and maintenance entries

## Setup

1. Clone the repository using clasp:
```bash
clasp clone "1lVvFrEmVQl2Nc2ijTruldoTCae5eZdE_gOsnPxmHISLXgnvdKFV3n418"
```

2. Install dependencies:
```bash
npm install -g @google/clasp
```

3. Login to clasp:
```bash
clasp login
```

## Development

- `index.html`: Main web interface
- `server/`: Backend logic
  - `Server.js`: Main server logic
  - `Backend.js`: Backend functions
  - `Helpers.js`: Utility functions
  - `Middleware.js`: Request middleware
  - `env.js`: Environment configuration

## Deployment

The application is deployed as a Google Apps Script web app with the following configuration:
- Execute as: User deploying the web app
- Access: Anyone, even anonymous
- Timezone: Africa/Cairo
- Mobile-optimized delivery

## Dependencies

- Google Sheets API v4
- AFILibrary (Development Mode)
- AFI Controller Library (Database operations)

## Contributing

1. Make your changes
2. Test thoroughly
3. Push changes using clasp:
```bash
clasp push
```

## Support

For system support, contact the IT department at support@advancedfoodindustries.com

## License

Proprietary - Advanced Food Industries (AFI) 