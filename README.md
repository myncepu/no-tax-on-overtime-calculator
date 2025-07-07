# No Tax on Overtime Calculator

A fast, private, and user-friendly calculator for estimating potential federal tax deductions under the U.S. No Tax on Overtime Act. Built with vanilla HTML, CSS, and JavaScript for maximum performance and privacy.

🔗 **Live Demo**: [notaxonovertimecalculator.org](https://notaxonovertimecalculator.org)

## 📋 Overview

The No Tax on Overtime Calculator helps workers estimate how much of their overtime premium pay may be tax-free under the No Tax on Overtime Act (effective 2025-2028). The tool provides instant calculations with clear explanations, all while respecting user privacy by performing calculations entirely client-side.

## ✨ Features

### 🧮 Core Calculator
- **Instant Calculations**: Real-time overtime tax deduction estimates
- **FLSA Compliance**: Only calculates the overtime premium (0.5x rate) that qualifies
- **Income Phase-outs**: Automatically applies income-based deduction reductions
- **Filing Status Support**: Handles both Single and Married Filing Jointly

### 🎨 Modern Interface
- **Responsive Design**: Works seamlessly on desktop and mobile
- **Clean UI**: Modern card-based layout with intuitive form fields
- **Accessibility**: Proper labeling and keyboard navigation support

### 🔒 Privacy-First
- **No Data Collection**: All calculations performed locally in browser
- **No Cookies**: Zero tracking or persistent storage
- **No Third-party Scripts**: Minimal external dependencies (only Plausible analytics)

### 📚 Educational Content
- **Comprehensive Guide**: Step-by-step usage instructions
- **Legal Context**: Explanation of the No Tax on Overtime Act
- **FAQ Section**: Common questions and answers
- **Real-world Examples**: Practical scenarios and calculations

### 📧 User Engagement
- **Email Updates**: Google Forms integration for feature announcements
- **Update Notifications**: Stay informed about regulation changes

## 🚀 Quick Start

### Prerequisites
- A modern web browser
- Basic web server (for local development)

### Local Development
```bash
# Clone the repository
git clone https://github.com/myncepu/no-tax-on-overtime-calculator.git

# Navigate to project directory
cd no-tax-on-overtime-calculator

# Serve locally (choose one method)
# Option 1: Python
python -m http.server 8000

# Option 2: Node.js
npx serve .

# Option 3: PHP
php -S localhost:8000

# Open browser
open http://localhost:8000
```

## 📁 Project Structure

```
no-tax-on-overtime-calculator/
├── index.html          # Main calculator page
├── terms.html          # Terms of Service
├── privacy.html        # Privacy Policy
├── README.md           # Project documentation
└── .gitignore         # Git ignore file
```

## 🎯 How It Works

### Tax Calculation Logic
The calculator implements the No Tax on Overtime Act formula:

1. **Calculate Overtime Premium**: `(Hourly Rate × 0.5) × Overtime Hours`
2. **Apply Deduction Cap**: 
   - Single: $12,500
   - Married Filing Jointly: $25,000
3. **Apply Income Phase-out**:
   - Phase-out starts at $150k (Single) / $300k (Joint)
   - Reduction: $100 for every $1,000 over threshold
4. **Final Deduction**: `Min(Premium, Adjusted Cap)`

### Example Calculation
```javascript
// Single filer, $80k MAGI, $25/hour, 400 OT hours
const premium = 25 * 0.5 * 400;        // $5,000
const cap = 12500;                      // No phase-out (under $150k)
const deduction = Math.min(5000, 12500); // $5,000
```

## 🛠️ Technology Stack

- **Frontend**: Vanilla HTML5, CSS3, JavaScript (ES6+)
- **Analytics**: Plausible (privacy-focused)
- **Email Collection**: Google Forms
- **Hosting**: Static site hosting compatible
- **No Build Process**: Direct browser execution

## 🚀 Deployment

### Static Site Hosts
The project works with any static site hosting service:

- **Netlify**: Drag and drop deployment
- **Vercel**: Git-based deployment
- **GitHub Pages**: Direct from repository
- **Cloudflare Pages**: Fast global CDN

### Custom Domain Setup
1. Point domain to hosting provider
2. Update Plausible analytics domain setting
3. Update Google Forms domain (if applicable)

## 🤝 Contributing

We welcome contributions! Here's how you can help:

### Types of Contributions
- 🐛 Bug fixes
- ✨ New features
- 📝 Documentation improvements
- 🎨 UI/UX enhancements
- 🧪 Test coverage

### Development Process
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Code Standards
- Use semantic HTML
- Follow existing CSS methodology
- Write vanilla JavaScript (no frameworks)
- Maintain browser compatibility
- Test on multiple devices

## 📜 Legal Compliance

### Tax Calculations
- Based on publicly available No Tax on Overtime Act text
- Educational estimates only - not professional tax advice
- Users advised to consult qualified tax professionals

### Data Privacy
- No personal data collection
- GDPR and CCPA compliant by design
- Transparent privacy policy

## 📈 Analytics & Monitoring

- **Plausible Analytics**: Privacy-focused visitor tracking
- **Performance**: Lighthouse scoring for web vitals
- **Uptime**: Static hosting for 99.9% availability

## 🔄 Update Process

### Regulation Changes
1. Monitor IRS and Treasury guidance
2. Update calculation logic as needed
3. Notify email subscribers
4. Update documentation

### Feature Updates
1. Test thoroughly across browsers
2. Update this README
3. Tag releases for version tracking

## 📞 Support

- **Email**: [support@notaxonovertimecalculator.org](mailto:support@notaxonovertimecalculator.org)
- **Issues**: [GitHub Issues](https://github.com/myncepu/no-tax-on-overtime-calculator/issues)
- **Discussions**: [GitHub Discussions](https://github.com/myncepu/no-tax-on-overtime-calculator/discussions)

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## ⚠️ Disclaimer

This calculator provides educational estimates only and is not legal, tax, or financial advice. Due to limited public guidance on the No Tax on Overtime Act, calculations may contain errors or omissions. Always consult a qualified tax professional before making tax-related decisions.

---

**Made with ❤️ in the USA** | [Website](https://notaxonovertimecalculator.org) | [GitHub](https://github.com/myncepu/no-tax-on-overtime-calculator) 