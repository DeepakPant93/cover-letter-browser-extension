# Cover Letter Generator Chrome Extension

A Chrome browser extension that automatically generates personalized cover letters based on job postings and your professional profiles.

## Overview

This extension analyzes job postings across various job portals and uses the information from your professional profiles (LinkedIn, GitHub, personal website, LeetCode, and resume) to create tailored cover letters that highlight your relevant skills and experiences.

## Features

- **One-Click Cover Letter Generation**: Generate a customized cover letter with a single click while browsing job postings
- **Profile Integration**: Connect your professional profiles to enhance cover letter personalization
- **Multi-Platform Support**: Works across major job portal websites
- **Secure Authentication**: Email verification ensures the security of your account
- **Instant Download**: Download your generated cover letter immediately

## Installation

1. Download the extension from the Chrome Web Store (link coming soon)
2. Click "Add to Chrome" to install the extension
3. Create an account and set up your profile
4. Start browsing job listings and generate your cover letters

## Getting Started

### Account Creation

1. Click on the extension icon after installation
2. Click "Sign Up" to create a new account
3. Enter your email address and create a password
4. Verify your email address through the verification link sent to your inbox

### Profile Setup

After verifying your email, you'll need to set up your profile with the following information:

- **Required**:
  - First Name
  - Last Name
  - LinkedIn Profile URL
  - Resume Link (Google Drive or GitHub)
  
- **Optional**:
  - Middle Name
  - GitHub Profile URL
  - Personal Website URL
  - LeetCode Profile URL

### Using the Extension

1. Navigate to any supported job portal
2. Find a job posting you're interested in
3. Click the Cover Letter Generator extension icon in your browser toolbar
4. Wait a few seconds while the AI analyzes the job posting and your profile
5. Review the generated cover letter
6. Download the cover letter as a document

## How It Works

1. The extension extracts key information from the job posting
2. It sends this information along with your profile links to our AI service
3. Google Gemini API analyzes the content and creates a personalized cover letter
4. The generated cover letter is presented for your review and download

## Supported Job Portals

- LinkedIn Jobs
- Indeed
- Glassdoor
- Monster
- ZipRecruiter
- And more...

## Security & Privacy

- Your profile information is securely stored and encrypted
- We do not share your information with third parties
- You maintain full control over which profiles you connect
- Cover letters are generated using Google Gemini API

## Technical Requirements

- Chrome browser version 88 or higher
- Active internet connection
- Valid email address for account verification

## Troubleshooting

If you encounter any issues:

1. Ensure you've completed your profile setup with all required fields
2. Verify that your profile links are valid and accessible
3. Make sure you're on a supported job portal website
4. Check that you're logged into your account

For additional support, please contact us at support@coverlettergen.com

## Future Updates

- Support for additional browsers (Firefox, Edge)
- Cover letter templates selection
- Integration with more job portals
- Enhanced customization options

## Development

### Project Structure

```
├── manifest.json          # Extension configuration
├── background.js          # Background service worker
├── popup/                 # Extension popup interface
│   ├── popup.html
│   ├── popup.css
│   └── popup.js
├── content/               # Content scripts for job portal integration
│   ├── content.js
│   └── parser.js
├── auth/                  # Authentication services
│   ├── auth.js
│   └── profile.js
└── services/              # Core services
    ├── jobExtractor.js    # Job posting extraction
    ├── aiService.js       # Gemini API integration
    └── api.js             # API communication
```

### Technology Stack

- **Frontend**: HTML, CSS, JavaScript
- **Backend**: Python (FastAPI or Flask)
- **Database**: MongoDB
- **Authentication**: JWT
- **AI/ML**: Google Gemini API
- **Text Processing**: Python NLP libraries (NLTK, spaCy)

## Contributing

We welcome contributions to improve the Cover Letter Generator! Please follow these steps:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Contact

For questions, feedback, or support, please reach out to us at:
- Email: info@coverlettergen.com
- Twitter: @CoverLetterGen
