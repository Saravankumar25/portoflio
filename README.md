# 🚀 Modern React Portfolio Website

A visually stunning, high-performance personal portfolio website built with React, featuring dark theme with glassmorphism styling, smooth animations, and modern UI/UX design.

## ✨ Features

### 🎨 Design & UI
- **Dark Theme**: Modern dark design with elegant color schemes
- **Glassmorphism Effects**: Semi-transparent panels with backdrop blur
- **Responsive Design**: Mobile-first approach, works on all devices
- **Modern Typography**: Clean, professional font hierarchy
- **Smooth Animations**: GSAP and CSS-based animations throughout

### 🔧 Technical Features
- **React Functional Components**: Modern React with hooks
- **Smooth Scrolling**: Between sections with navigation highlights  
- **Loading Animation**: Professional loading screen
- **EmailJS Integration**: Functional contact form
- **SEO Optimized**: Meta tags and semantic HTML
- **Accessibility**: ARIA labels, keyboard navigation, semantic structure
- **Performance**: Optimized animations and lazy loading

### 📱 Sections
- **Hero Section**: Animated introduction with typing effects
- **About Me**: Timeline of education and personal statement
- **Skills**: Categorized technical skills with animated displays
- **Projects**: Interactive project gallery with filtering
- **Experience**: Educational timeline with achievements
- **Contact**: Functional contact form with validation

## 🛠️ Tech Stack

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Animations**: GSAP (GreenSock Animation Platform)
- **Styling**: CSS Custom Properties, Flexbox, Grid
- **Contact Form**: EmailJS integration
- **Icons**: Font Awesome (CDN)
- **Deployment**: GitHub Pages / Vercel ready

## 📁 Project Structure

```
portfolio-website/
├── index.html          # Main HTML file
├── style.css           # Comprehensive CSS with glassmorphism
├── app.js              # Main JavaScript with all functionality
├── README.md           # This file
├── assets/
│   ├── images/         # Profile and project images
│   └── icons/          # Custom SVG icons
└── components/
    ├── animations/     # Animation utilities
    ├── sections/       # Section-specific code
    └── ui/            # Reusable UI components
```

## 🚀 Quick Start

### Prerequisites
- Node.js (v14 or higher)
- Git
- Modern web browser

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/portfolio-website.git
   cd portfolio-website
   ```

2. **Install dependencies** (if using npm for development)
   ```bash
   npm install
   ```

3. **Configure EmailJS**
   - Sign up at [EmailJS](https://www.emailjs.com/)
   - Create a service and email template
   - Replace `YOUR_PUBLIC_KEY` in `app.js` with your EmailJS public key
   - Update service ID and template ID in the contact form section

4. **Development Server**
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   
   # Using VS Code Live Server extension
   # Right-click index.html → "Open with Live Server"
   ```

5. **Open in browser**
   ```
   http://localhost:8000
   ```

## 🌐 Deployment

### GitHub Pages

1. **Setup Repository**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/username/repository-name.git
   git push -u origin main
   ```

2. **Enable GitHub Pages**
   - Go to repository Settings → Pages
   - Select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Save and wait for deployment

3. **Access your site**
   ```
   https://username.github.io/repository-name
   ```

### Vercel Deployment

1. **Install Vercel CLI**
   ```bash
   npm install -g vercel
   ```

2. **Deploy**
   ```bash
   vercel login
   vercel
   ```

3. **Follow prompts and deploy**
   - Your site will be live with a `.vercel.app` domain
   - Connect custom domain if needed

### Alternative Deployment Options
- **Netlify**: Drag and drop the folder to Netlify dashboard
- **Firebase Hosting**: Use Firebase CLI for deployment
- **Surge.sh**: Simple command-line deployment

## ⚙️ Configuration

### EmailJS Setup
1. Create account at EmailJS
2. Set up email service (Gmail, Outlook, etc.)
3. Create email template
4. Get your public key and service/template IDs
5. Update in `app.js`:
   ```javascript
   emailjs.init("YOUR_PUBLIC_KEY");
   // Update service and template IDs in sendEmail function
   ```

### Customization

#### Personal Information
Update the data object in `app.js` with your information:
```javascript
const personalData = {
    name: "Your Name",
    title: "Your Title",
    email: "your.email@domain.com",
    // ... other details
};
```

#### Color Theme
Modify CSS custom properties in `style.css`:
```css
:root {
    --primary-color: #your-color;
    --accent-color: #your-accent;
    /* ... other colors */
}
```

#### Projects & Skills
Update the projects and skills arrays in `app.js` with your own data.

## 🎨 Design System

### Color Palette
- **Background**: Deep dark (#0a0a0a)
- **Surface**: Dark gray (#111111)
- **Primary**: Electric blue (#00d4ff)
- **Accent**: Purple gradient (#8b5cf6)
- **Text**: Light gray (#e5e5e5)

### Typography
- **Headings**: Inter, system-ui
- **Body**: -apple-system, BlinkMacSystemFont
- **Code**: 'Fira Code', monospace

### Animations
- **Duration**: 0.3s - 0.8s for transitions
- **Easing**: cubic-bezier for smooth motion
- **Triggers**: Intersection Observer for scroll animations

## 📱 Responsive Breakpoints

```css
/* Mobile */
@media (max-width: 640px) { ... }

/* Tablet */
@media (max-width: 768px) { ... }

/* Laptop */
@media (max-width: 1024px) { ... }

/* Desktop */
@media (max-width: 1280px) { ... }
```

## ♿ Accessibility Features

- **Semantic HTML**: Proper heading hierarchy and landmarks
- **ARIA Labels**: Screen reader friendly navigation
- **Keyboard Navigation**: Full keyboard support
- **Color Contrast**: WCAG 2.1 AA compliant
- **Focus Management**: Visible focus indicators
- **Alt Text**: All images have descriptive alt text

## 🔧 Browser Support

- **Chrome**: 88+
- **Firefox**: 85+
- **Safari**: 14+
- **Edge**: 88+

## 📈 Performance Optimizations

- **CSS**: Minified and optimized
- **JavaScript**: Efficient event handling and animations
- **Images**: Optimized formats and lazy loading
- **Fonts**: System fonts with web font fallbacks
- **Animations**: Hardware accelerated transforms

## 🐛 Troubleshooting

### Common Issues

1. **EmailJS not working**
   - Check public key configuration
   - Verify service and template IDs
   - Check browser console for errors

2. **Animations not smooth**
   - Ensure GSAP is loaded before script execution
   - Check for JavaScript errors in console

3. **Mobile navigation issues**
   - Clear browser cache
   - Check viewport meta tag

4. **GitHub Pages deployment issues**
   - Ensure repository name matches GitHub username
   - Check Pages settings in repository

## 🤝 Contributing

1. Fork the repository
2. Create feature branch (`git checkout -b feature/amazing-feature`)
3. Commit changes (`git commit -m 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing-feature`)
5. Open Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Saravan Kumar M K**
- Email: saravankumar2503@gmail.com
- LinkedIn: [saravan-kumar-m-k](https://linkedin.com/in/saravan-kumar-m-k-35014a220)
- GitHub: [Saravankumar25](https://github.com/Saravankumar25)

## 🙏 Acknowledgments

- **GSAP**: For powerful animation capabilities
- **EmailJS**: For seamless contact form integration
- **Font Awesome**: For beautiful icons
- **Unsplash**: For high-quality placeholder images
- **CSS Glassmorphism**: For modern design inspiration

## 📚 Resources

- [GSAP Documentation](https://greensock.com/docs/)
- [EmailJS Documentation](https://www.emailjs.com/docs/)
- [MDN Web Docs](https://developer.mozilla.org/)
- [CSS Tricks](https://css-tricks.com/)
- [React Documentation](https://reactjs.org/docs/)

---

⭐ **If you like this project, please give it a star!** ⭐

Made with ❤️ and modern web technologies