# Backable Finance Engine

## Your Financial Command Center

A comprehensive web-based financial assessment platform that helps businesses analyze their financial health, track performance, and make data-driven decisions through interactive assessments and AI-powered document analysis.

![Backable Finance Engine](https://img.shields.io/badge/Finance-Engine-blue?style=for-the-badge)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow?style=flat-square)
![HTML5](https://img.shields.io/badge/HTML5-Modern-orange?style=flat-square)
![CSS3](https://img.shields.io/badge/CSS3-Responsive-blue?style=flat-square)

## 🌟 Key Features

### 📊 Interactive Financial Assessments
- **Financial Foundation Assessment**: Establish your baseline financial truth and operating system
- **Financial Mastery Assessment**: Dive deep into advanced financial strategies and optimization
- **Financial Intelligence Assessment**: Unlock strategic insights and predictive analytics

### 📁 AI-Powered Document Processing
- **Multi-Category Document Upload**: Support for Profit & Loss, Balance Sheets, Income Statements, Management Reports, Budget Analysis, and Supporting Documents
- **Real-time Processing**: Live status updates and extraction progress tracking
- **Smart Data Extraction**: AI-powered analysis of financial documents with field recognition

### 🎯 Advanced Question Types
- **Card-Based Selections**: Intuitive choice interfaces with conditional follow-ups
- **Financial Tables**: Dynamic revenue projections and historical data entry
- **Slider Controls**: Precise value selection with real-time feedback
- **Matrix Sliders**: Multi-dimensional assessment inputs
- **Ranking Systems**: Drag-and-drop prioritization
- **Checkbox Options**: Multi-selection with limits

### 💾 Real-Time Data Management
- **Auto-Save Functionality**: Automatic progress preservation
- **Session Tracking**: Comprehensive metadata collection and timing analysis
- **Progress Monitoring**: Visual progress indicators and completion tracking
- **Data Persistence**: Secure backend storage with recovery capabilities

### 🔗 Backend Integration
- **RESTful API Communication**: Seamless connection to backend services
- **Connection Monitoring**: Real-time backend connectivity status
- **Error Handling**: Robust error management and user feedback
- **File Processing Jobs**: Asynchronous document processing with status tracking

## 🚀 Quick Start

### Prerequisites
- Modern web browser (Chrome 90+, Firefox 88+, Safari 14+)
- Backend API server running on `http://localhost:8001` (configurable)
- Internet connection for backend communication

### Installation
1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd backable-finance-engine-polling
   ```

2. **Open the application**
   - Open `BACKABLE FINANCE ENGINE POLLING.html` in your web browser
   - No additional setup required - it's a self-contained HTML application

3. **Configure Backend (Optional)**
   - Update `API_BASE_URL` in the script section if your backend runs on a different port
   - Default: `http://localhost:8001`

## 📋 Usage Guide

### 1. Initial Setup
- Enter your business name, revenue range, and growth target
- The system will personalize questions based on your inputs

### 2. Assessment Selection
Choose from three assessment types:
- **Foundation**: Basic financial health and systems assessment
- **Mastery**: Advanced financial strategies and optimization
- **Intelligence**: Strategic insights and predictive analysis

### 3. Document Upload
Upload financial documents by category:
- **Profit & Loss Statements**: Last 2 years + YTD
- **Balance Sheets**: Assets, liabilities, and equity statements
- **Income Statements**: Detailed expense analysis
- **Management Reports**: Monthly/quarterly internal reports
- **Budget vs Actual**: Variance analysis reports
- **Supporting Documents**: Additional financial analysis files

### 4. Interactive Assessment
Navigate through questions using various input methods:
- Click card options for quick selections
- Use sliders for precise value input
- Fill financial tables with historical and projected data
- Drag and drop for ranking priorities

### 5. Progress Tracking
- Monitor completion status with visual progress bars
- Auto-save ensures no progress is lost
- Review and modify responses as needed

## 🛠️ Technical Architecture

### Frontend Technologies
- **HTML5**: Semantic markup with modern features
- **CSS3**: Responsive design with gradients and animations
- **Vanilla JavaScript (ES6+)**: No framework dependencies
- **Progressive Web App Features**: Offline-capable, responsive design

### Core Components
- **FinanceEngine Object**: Central orchestration engine
- **Assessment System**: Modular question management
- **File Processing Engine**: Document upload and analysis
- **Progress Management**: Session and response tracking
- **Backend Communication**: API integration layer

### Key Functions
- `selectAssessment()`: Assessment type selection
- `showQuestion()`: Dynamic question rendering
- `processFiles()`: Document upload processing
- `saveProgressToBackend()`: Data persistence
- `checkBackendConnection()`: Connectivity monitoring

## 🔧 Configuration

### Backend Configuration
```javascript
const API_BASE_URL = "http://localhost:8001"; // Change this for different environments
```

### Document Categories
The system supports 6 document categories with configurable limits:
- Max 3 files per category for most types
- Max 5 files for management reports
- Max 10 files for supporting documents

### Assessment Structure
Each assessment contains multiple sections with varied question types:
- Card selections with conditional logic
- Financial data tables
- Slider-based inputs
- Ranking systems
- Text inputs with character limits

## 📊 Data Flow

1. **User Input Collection**: Interactive form responses
2. **Document Processing**: File upload → AI extraction → Data storage
3. **Progress Tracking**: Real-time session metadata collection
4. **Backend Synchronization**: Auto-save and data persistence
5. **Results Generation**: Assessment completion and insights delivery

## 🎨 UI/UX Features

- **Responsive Design**: Works on desktop, tablet, and mobile
- **Modern Aesthetics**: Gradient backgrounds and smooth animations
- **Intuitive Navigation**: Clear progress indicators and breadcrumbs
- **Accessibility**: Keyboard navigation and screen reader support
- **Visual Feedback**: Loading states, success/error messages

## 🔍 Debug Features

Access debug functions via browser console:
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

## 🚨 Troubleshooting

### Common Issues

**Backend Connection Failed**
- Verify backend server is running on port 8001
- Check network connectivity
- Review browser console for detailed error messages

**File Upload Issues**
- Ensure files are in supported formats (PDF, images, documents)
- Check file size limits
- Verify backend file processing endpoints

**Assessment Progress Not Saving**
- Check auto-save functionality
- Verify backend storage endpoints
- Review browser local storage

### Browser Compatibility
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📝 License

This project is proprietary software. All rights reserved.

## 🆘 Support

For technical support or questions:
- Check the debug console for error messages
- Review network requests in browser dev tools
- Ensure backend services are properly configured

## 🔄 Version History

- **Current Version**: 1.0.0
- Single-page application with full financial assessment capabilities
- AI-powered document processing integration
- Real-time backend synchronization

---