# Leap API Documentation

This repository contains the complete API documentation for the Leap platform, built with Swagger UI and deployed on GitHub Pages.

## 🚀 Live Documentation

The documentation is automatically deployed to GitHub Pages and available at:
**https://[your-username].github.io/swagger-test/**

## 📁 Project Structure

```
├── index.html                 # Main Swagger UI documentation page
├── public/
│   └── swagger/
│       ├── index.html         # Alternative Swagger UI page
│       └── api/
│           ├── index.json     # API index configuration
│           ├── introduction.json  # API introduction and overview
│           └── customer.json  # Customer API specification
└── .github/
    └── workflows/
        └── pages.yml          # GitHub Pages deployment workflow
```

## 🔧 Setup Instructions

### For GitHub Pages Deployment:

1. **Enable GitHub Pages:**
   - Go to your repository settings
   - Navigate to "Pages" section
   - Select "GitHub Actions" as the source

2. **Push to main branch:**
   - The workflow will automatically deploy your documentation
   - Check the "Actions" tab for deployment status

3. **Access your documentation:**
   - Visit `https://[your-username].github.io/swagger-test/`

### Local Development:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/[your-username]/swagger-test.git
   cd swagger-test
   ```

2. **Serve locally:**
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   
   # Using PHP
   php -S localhost:8000
   ```

3. **Open in browser:**
   - Navigate to `http://localhost:8000`

## 📚 API Documentation Features

- **Interactive API Explorer**: Test endpoints directly from the documentation
- **Authentication Support**: Bearer token authentication
- **Comprehensive Examples**: Request/response examples for all endpoints
- **Search and Filter**: Advanced querying capabilities
- **Mobile Responsive**: Optimized for all device sizes

## 🔑 API Endpoints

### Customer Management
- `GET /customers` - Retrieve all customers
- `POST /customers` - Create a new customer
- `GET /customers/{id}` - Get customer details
- `PUT /customers/{id}` - Update customer information

## 🛠️ Customization

### Adding New API Specifications:

1. Create a new JSON file in `public/swagger/api/`
2. Update `public/swagger/api/index.json` to include the new specification
3. The documentation will automatically include the new endpoints

### Modifying the UI:

1. Edit `index.html` to customize the Swagger UI appearance
2. Modify the CSS styles in the `<style>` section
3. Update the JavaScript configuration as needed

## 📝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test locally
5. Submit a pull request

## 📄 License

This documentation is provided as-is for the Leap platform API.

## 🆘 Support

For API support or questions about the documentation, please contact the development team.
