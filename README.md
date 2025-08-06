# Password Security Checker 🔐

A modern, responsive web application that helps users evaluate the strength and security of their passwords in real-time. The tool provides instant feedback on password strength and checks against known data breaches using the HaveIBeenPwned API.

## Features

### 🔍 Real-time Password Analysis
- **Strength Meter**: Visual indicator showing password strength from weak to strong
- **Character Requirements**: Checks for lowercase, uppercase, numbers, and special characters
- **Length Validation**: Ensures passwords meet minimum length requirements
- **Pattern Detection**: Identifies common sequences (123, abc, qwe) and repeating characters

### 🛡️ Security Features
- **Breach Database Check**: Securely checks passwords against the HaveIBeenPwned database
- **Privacy-First**: Uses SHA-1 hashing with k-anonymity (only first 5 characters of hash are sent)
- **Password Visibility Toggle**: Option to show/hide password while typing
- **No Data Storage**: All processing happens locally in the browser

### 📱 Responsive Design
- **Mobile-Optimized**: Fully responsive design that works on all screen sizes
- **Touch-Friendly**: Large buttons and inputs optimized for mobile devices
- **Cross-Browser**: Compatible with modern web browsers
- **Accessibility**: Proper contrast ratios and semantic HTML

## How It Works

1. **Enter Password**: Type your password in the input field
2. **Real-time Analysis**: The tool immediately evaluates your password strength
3. **Visual Feedback**: A color-coded strength meter shows your password's security level
4. **Detailed Results**: Individual checks show which security criteria are met
5. **Breach Check**: The password is securely checked against known data breaches

## Password Strength Criteria

The tool evaluates passwords based on:

- ✅ **Minimum 8 characters** (required)
- ✅ **12+ characters** (recommended)
- ✅ **Lowercase letters** (a-z)
- ✅ **Uppercase letters** (A-Z)
- ✅ **Numbers** (0-9)
- ✅ **Special characters** (!@#$%^&*()_+-=[]{}|;:,.<>?)
- ✅ **No common sequences** (123, abc, qwe)
- ✅ **No repeating characters** (aaa, 111)

## Strength Levels

- 🔴 **Weak** (0-3 criteria): High risk, easy to crack
- 🟡 **Fair** (4-5 criteria): Moderate security
- 🟢 **Good** (6-7 criteria): Strong security
- 🔵 **Strong** (8 criteria): Excellent security

## Privacy & Security

- **No Data Transmission**: Your full password never leaves your browser
- **Secure Hashing**: Uses SHA-1 hashing for breach database queries
- **K-Anonymity**: Only the first 5 characters of the hash are sent to the API
- **HTTPS Required**: Breach database checks use secure HTTPS connections

## Technical Details

- **Pure HTML/CSS/JavaScript**: No external dependencies
- **Modern Web APIs**: Uses Web Crypto API for secure hashing
- **Responsive CSS**: Mobile-first design with flexbox and CSS Grid
- **Debounced Input**: 300ms delay prevents excessive API calls
- **Error Handling**: Graceful fallback when network requests fail

## Browser Compatibility

- Chrome 60+
- Firefox 55+
- Safari 11+
- Edge 79+

## Usage

Simply open [index.html](index.html) in any modern web browser. No installation or server setup required.

## API Credits

This tool uses the [HaveIBeenPwned Pwned Passwords API](https://haveibeenpwned.com/API/v3#PwnedPasswords) by Troy Hunt to check passwords against known data breaches.

## License

This project is open source and available under the MIT License.
