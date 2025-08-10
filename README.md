# API Gina Plus - Product Status Update Tool

A web-based tool for updating product statuses via API using Excel/CSV files.

## Features

- Upload Excel/CSV files with product data
- Configure API endpoints and authentication headers
- Batch update product statuses via REST API
- Support for multiple HTTP methods (POST, PUT, PATCH)
- Custom header configuration
- Local storage for saving settings
- Concurrent API request handling with rate limiting

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
