# Backable Finance Engine

A web-based financial assessment platform with interactive questionnaires and AI-powered document processing.

## Setup

### Prerequisites
- Modern web browser (Chrome 90+, Firefox 88+, Safari 14+, Edge 90+)
- Backend API server running on `http://localhost:8001`

### Installation
1. Clone the repository
2. Open `BACKABLE FINANCE ENGINE POLLING.html` in your web browser

### Configuration
Update `API_BASE_URL` in the script section for different backend endpoints:
```javascript
const API_BASE_URL = "http://localhost:8001";
```

## Usage

### Initial Setup
1. Enter business name, revenue range, and growth target
2. Select assessment type (Foundation, Mastery, or Intelligence)

### Document Upload
Upload financial documents by category:
- Profit & Loss Statements
- Balance Sheets
- Income Statements
- Management Reports
- Budget vs Actual Reports
- Supporting Documents

File limits: 3 per category (5 for management reports, 10 for supporting documents)

### Assessment Flow
Navigate through questions using:
- Card selections with conditional logic
- Financial data tables
- Slider controls
- Matrix sliders
- Ranking systems (drag-and-drop)
- Text inputs with character limits

## Technical Architecture

### Technologies
- HTML5, CSS3, JavaScript (ES6+)
- No external dependencies
- Single-page application

### Core Components
- `FinanceEngine`: Main orchestration object
- Assessment system with modular questions
- File processing with AI extraction
- Backend API integration
- Auto-save functionality

### Key Functions
- `selectAssessment()`: Choose assessment type
- `showQuestion()`: Render questions dynamically
- `processFiles()`: Handle document uploads
- `saveProgressToBackend()`: Persist data
- `checkBackendConnection()`: Monitor connectivity

## Debug Features

Access via browser console:
```javascript
// Get current responses
financeDebug.getResponses()

// View uploaded files summary
financeDebug.getUploadedFilesSummary()

// Check backend connection
financeDebug.checkConnection()

// Clear all responses
financeDebug.clearAllResponses()
```

## Troubleshooting

### Backend Connection Issues
- Verify backend server is running on port 8001
- Check network connectivity
- Review browser console for errors

### File Upload Issues
- Ensure supported formats (PDF, images, documents)
- Check file size limits
- Verify backend file processing endpoints

### Progress Not Saving
- Check auto-save functionality
- Verify backend storage endpoints