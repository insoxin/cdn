# Error Pages - Complete Collection

This repository now includes a complete set of HTTP error pages designed in the style of Cloudflare, with all content in English.

## Pages Created

### Client Errors (4xx)

- **400.html** - Bad Request
  - For malformed request syntax or invalid parameters
  
- **401.html** - Unauthorized
  - For missing or invalid authentication credentials
  
- **403.html** - Forbidden
  - For access restriction issues
  
- **404.html** - Not Found
  - For missing or deleted resources
  
- **405.html** - Method Not Allowed
  - For unsupported HTTP methods
  
- **408.html** - Request Timeout
  - For requests that take too long
  
- **429.html** - Too Many Requests
  - For rate limiting violations

### Server Errors (5xx)

- **500.html** - Internal Server Error
  - For unexpected server conditions
  
- **502.html** - Bad Gateway
  - For invalid upstream responses
  
- **503.html** - Service Unavailable
  - For maintenance or overload situations
  
- **504.html** - Gateway Timeout
  - For upstream server timeout issues

## Design Features

### Modern Cloudflare-Style Design
- **Color Scheme**: Purple gradient background (#667eea to #764ba2)
- **Layout**: Centered white container with shadow
- **Typography**: Modern system fonts (-apple-system, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif)
- **Icons**: Unicode emoji icons for visual communication

### Key Sections
1. **Error Icon**: Relevant emoji for the error type
2. **Error Code**: Large, prominent error number
3. **Error Title**: Clear, descriptive error name
4. **Description**: User-friendly explanation
5. **What Can You Do?**: Actionable suggestions list
6. **Action Buttons**: 
   - Primary: "Go to Home" button
   - Secondary: "Go Back" button
7. **Footer**: Support contact information and error ID

### Responsive Design
- Mobile-friendly layout with media queries
- Adapts to screens 600px and below
- Touch-friendly button sizes

## Customization Options

Each page can be customized by modifying:
- Email address in support link (currently: support@example.com)
- Homepage URL (currently: /)
- Color scheme (currently: #667eea)
- Brand name or logo
- Support contact information

## Technical Details

- **Format**: HTML5 with embedded CSS
- **Language**: English
- **Charset**: UTF-8
- **Auto-refresh**: 360 seconds (6 minutes)
- **Viewport**: Responsive design

## Usage

Simply map these HTML files to their corresponding HTTP error codes in your web server configuration:

### Apache (.htaccess)
```
ErrorDocument 400 /400.html
ErrorDocument 401 /401.html
ErrorDocument 403 /403.html
ErrorDocument 404 /404.html
ErrorDocument 405 /405.html
ErrorDocument 408 /408.html
ErrorDocument 429 /429.html
ErrorDocument 500 /500.html
ErrorDocument 502 /502.html
ErrorDocument 503 /503.html
ErrorDocument 504 /504.html
```

### Nginx (nginx.conf)
```
error_page 400 /400.html;
error_page 401 /401.html;
error_page 403 /403.html;
error_page 404 /404.html;
error_page 405 /405.html;
error_page 408 /408.html;
error_page 429 /429.html;
error_page 500 /500.html;
error_page 502 /502.html;
error_page 503 /503.html;
error_page 504 /504.html;
```

---

**Created**: 2026-05-30
**Version**: 1.0
**Language**: English
**Design**: Cloudflare-inspired
