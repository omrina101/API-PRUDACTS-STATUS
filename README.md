# API Gina Plus - Product Status Update Tool

A web-based tool for updating product statuses via API using Excel/CSV files.

**Current Version:** v1.0.0  
**Build Number:** 1  
**Last Update:** Today

## 🚀 Version Management System

This application includes an automatic version management system that tracks:
- **Semantic Versioning** (Major.Minor.Patch)
- **Build Numbers** (auto-incremented)
- **Update History** with change logs
- **Automatic Version Updates** after PUSH operations

### How to Update Versions

#### Option 1: Automatic Update (Recommended)
After each PUSH to your repository, run in the browser console:
```javascript
versionControl.autoIncrement()
```

#### Option 2: Manual Version Control
```javascript
// Increment patch version (1.0.0 → 1.0.1)
versionControl.increment('patch')

// Increment minor version (1.0.0 → 1.1.0)
versionControl.increment('minor')

// Increment major version (1.0.0 → 2.0.0)
versionControl.increment('major')

// Set specific version
versionControl.advanced('set', '1.2.3', ['New feature added', 'Bug fixes'])
```

#### Option 3: Advanced Operations
```javascript
// Export version configuration
versionControl.advanced('export')

// Reset build number
versionControl.advanced('reset')

// Get current version info
versionControl.getCurrent()
versionControl.getBuild()
versionControl.getHistory()
```

## Features

- Upload Excel/CSV files with product data
- Configure API endpoints and authentication headers
- Batch update product statuses via REST API
- Support for multiple HTTP methods (POST, PUT, PATCH)
- Custom header configuration
- Local storage for saving settings
- Concurrent API request handling with rate limiting
- **NEW:** Automatic version management and tracking
- **NEW:** Build number tracking
- **NEW:** Update history with change logs

## Usage

1. Open `index.html` in your web browser
2. Configure your API endpoint and authentication headers
3. Test the API connection
4. Upload your Excel/CSV file
5. Review the data and start the update process

## File Format

Your Excel/CSV file should contain:
- Product SKU or identifier
- Status field to update
- Any other required fields for your API

## API Configuration

- **API URL**: Your endpoint for updating products
- **Method**: HTTP method (POST, PUT, PATCH)
- **Authentication Header**: Header name and value for API authentication
- **Extra Headers**: Additional headers in JSON format

## Deployment

This project can be deployed to:
- GitHub Pages
- Netlify
- Vercel
- Any static hosting service

## Browser Compatibility

- Modern browsers with ES6+ support
- Requires JavaScript enabled
- File API support for Excel/CSV uploads

## Version History

### v1.0.0 (Initial Release)
- Initial version
- Excel/CSV support
- API integration
- CORS proxy support
- Version management system
- Build tracking
- Update history

## Development Workflow

1. **Make Changes** to your code
2. **Test** the application
3. **Commit** your changes
4. **Push** to repository
5. **Update Version** using `versionControl.autoIncrement()`
6. **Deploy** the updated version

The version management system automatically:
- Increments build numbers
- Tracks update dates
- Maintains version history
- Updates the UI display
- Saves configuration to localStorage
