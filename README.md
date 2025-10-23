# Amazon Homepage Clone

A pixel-perfect replica of Amazon's homepage, built with pure HTML and CSS. This project demonstrates advanced CSS techniques, responsive design principles, and attention to detail in recreating a complex e-commerce interface.

## 📋 Table of Contents

- [Overview](#overview)
- [Live Demo](#live-demo)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [CSS Architecture](#css-architecture)
- [Key Components](#key-components)
- [Browser Compatibility](#browser-compatibility)
- [Responsive Design](#responsive-design)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)

## 🎯 Overview

This project is a faithful recreation of Amazon's homepage interface, built entirely from scratch using semantic HTML5 and modern CSS3. It showcases professional front-end development skills including layout design, component architecture, and pixel-perfect implementation with full responsive support for desktop, tablet, and mobile devices.

## 🌐 Live Demo

**[View Live Demo →](https://amazon-clone-one-coral.vercel.app)**

Deployed on Vercel with automatic HTTPS and global CDN distribution.

## ✨ Features

### Navigation System
- **Primary Navigation Bar**
  - Responsive logo and branding
  - Location selector with delivery information
  - Full-featured search bar with category dropdown
  - Language selector with country flag
  - User account section
  - Returns & Orders tracking
  - Shopping cart with item counter

- **Secondary Navigation**
  - Category menu with hamburger icon
  - Quick links to major sections
  - Hover effects and transitions
  - Horizontal scroll on mobile devices

### Main Content
- **Hero Section**
  - Full-width banner image
  - Gradient fade effect for seamless content integration
  - Responsive height adjustments

- **Product Cards Grid**
  - Responsive grid layout (3 columns → 2 columns → 1 column)
  - Six unique product category cards
  - Dynamic grid layouts (1x1, 2x2, 3x2)
  - Image hover effects
  - Call-to-action links with hover states

- **Personalization Section**
  - Sign-in recommendation card
  - New customer registration prompt

### Footer Architecture
- **Multi-tier Footer System**
  - "Back to Top" button
  - Comprehensive link sections (Get to Know Us, Make Money With Us, Payment Products, Help)
  - Amazon services and products grid
  - Legal and privacy information
  - Multi-column layout with 28+ service links
  - Language and region selector

### Design Features
- CSS custom properties (variables) for consistent theming
- Smooth transitions and hover effects (150ms ease)
- Professional spacing system (8px base)
- Typography hierarchy with Roboto font family
- Semantic HTML5 structure
- Pure HTML/CSS implementation (no JavaScript dependencies)
- Fully responsive design for all screen sizes

## 🛠 Technologies Used

- **HTML5** - Semantic markup and structure
- **CSS3** - Advanced styling and layout
  - Flexbox for navigation and components
  - CSS Grid for product card layouts
  - Custom Properties (CSS Variables)
  - Pseudo-elements for decorative effects
  - Advanced selectors and specificity
  - Media queries for responsive design
- **Google Fonts** - Roboto font family (400, 500, 700 weights)
- **Vercel** - Deployment and hosting

## 📁 Project Structure

```
amazon-clone/
│
├── index.html              # Main HTML file (semantic structure)
├── style.css               # Complete stylesheet with media queries
├── README.md               # Project documentation
│
└── Images/                 # Image assets
    ├── favicon.png         # Browser tab icon
    ├── logo.png            # Amazon logo sprite sheet
    ├── country-flag.png    # Flag icons sprite
    ├── hero.jpg            # Hero banner image
    ├── box1a.jpg - box1d.jpg    # Home essentials category
    ├── box2a.jpg - box2d.jpg    # Fashion items category
    ├── box3.jpg                  # Gaming category
    ├── box5a.jpg - box5d.jpg    # Kitchen appliances
    ├── box6a.jpg - box6d.jpg    # Space refresh category
    └── box8a.jpg - box8d.jpg    # Elevated spaces category
```

## 🚀 Installation

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- A code editor (VS Code recommended)
- Git (optional, for version control)

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/amazon-clone.git
   ```

2. **Navigate to the project directory**
   ```bash
   cd amazon-clone
   ```

3. **Open the project**
   - Simply open `index.html` in your web browser
   - Or use a local development server:
     ```bash
     # Using Python 3
     python -m http.server 8000
     
     # Using Node.js http-server
     npx http-server
     ```

4. **View in browser**
   - Direct: Double-click `index.html`
   - Local server: Navigate to `http://localhost:8000`

## 💻 Usage

### Viewing the Project
1. Open `index.html` in any modern web browser
2. Explore different sections and interactive hover effects
3. Resize browser window or use DevTools (F12) to test responsive breakpoints

### Customization

#### Changing Colors
Edit CSS custom properties in `style.css`:
```css
:root {
    --amazon-dark: #131921;
    --amazon-orange: #f08804;
    --amazon-yellow: #febd69;
    --amazon-light-bg: #f3f3f3;
    /* Modify these values to change the theme */
}
```

#### Modifying Content
Update product cards in `index.html`:
```html
<div class="cards">
    <p>Your Title Here</p>
    <div class="cards-content c1">
        <div class="card-item">
            <img src="Images/your-image.jpg" alt="Description">
            <span>Your Label</span>
        </div>
        <!-- Add more items -->
    </div>
    <a href="#">Your Link Text</a>
</div>
```

## 🎨 CSS Architecture

### Design System

#### Color Palette
```css
--amazon-dark: #131921      /* Primary navigation background */
--amazon-orange: #f08804    /* Accent color & hover states */
--amazon-yellow: #febd69    /* Search button & CTAs */
--amazon-light-bg: #f3f3f3  /* Card backgrounds */
--amazon-subnav: #232f3e    /* Secondary navigation */
--text-white: #ffffff       /* Primary text on dark */
--text-gray: #cccccc        /* Secondary text */
--text-footer: #DDDDDD      /* Footer links */
--text-dark: #333333        /* Body text */
```

#### Spacing System (8px base)
```css
--space-xs: 4px      /* Micro spacing */
--space-sm: 8px      /* Small spacing */
--space-md: 12px     /* Medium spacing */
--space-lg: 16px     /* Large spacing */
--space-xl: 24px     /* Extra large spacing */
--space-2xl: 32px    /* 2X large spacing */
--space-3xl: 39px    /* 3X large spacing */
```

#### Typography Scale
```css
--font-xs: 12px      /* Small text, captions */
--font-sm: 14px      /* Body text, labels */
--font-md: 16px      /* Headings, emphasis */
--font-lg: 18px      /* Large headings */
```

### Component Structure
- **Navbar**: Flexbox-based three-section layout (left, fill, right)
- **Cards Grid**: CSS Grid with flexible column templates
- **Footer**: Multi-column flex layout with wrapping
- **Transitions**: 150ms ease for smooth interactions

## 🔑 Key Components

### 1. Navigation Bar
- Fixed height (60px desktop, 50px mobile)
- Three-section flexbox layout
- Sprite-based icons for optimal performance
- Responsive search bar with category dropdown
- Collapsible elements on smaller screens

### 2. Product Cards
- Flexible grid layout (3 → 2 → 1 columns)
- Six unique grid templates (c1-c6) for varied layouts
- Hover shadow effects (0 4px 12px rgba)
- Responsive image containers with object-fit
- Dynamic height adjustments per breakpoint

### 3. Footer System
- Four-tier structure (content, bottom, end, legal)
- Dynamic link sections with flex wrapping
- Region/language selectors with flag sprites
- Comprehensive service and legal links
- Responsive stacking on mobile

### 4. Image Optimization
- **CSS Sprites**: All icons in single `logo.png` file
- **Flag Sprites**: Country flags in `country-flag.png`
- **Benefits**: Reduced HTTP requests, faster loading
- **Background positioning**: Precise pixel positioning

## 🌐 Browser Compatibility

| Browser | Version | Support |
|---------|---------|---------|
| Chrome  | 90+     | ✅ Full Support |
| Firefox | 88+     | ✅ Full Support |
| Safari  | 14+     | ✅ Full Support |
| Edge    | 90+     | ✅ Full Support |
| Opera   | 76+     | ✅ Full Support |

### CSS Features Used
- ✅ CSS Grid Layout
- ✅ Flexbox
- ✅ Custom Properties (CSS Variables)
- ✅ CSS Transitions
- ✅ Pseudo-elements (::before, ::after)
- ✅ Background sprites
- ✅ Media Queries
- ✅ Advanced Selectors

## 📱 Responsive Design

### Breakpoints
- **1024px and below** - Tablet/Small Desktop (2 cards per row)
- **768px and below** - Tablet Portrait (hidden elements, stacked footer)
- **640px and below** - Large Mobile (single column layout)
- **480px and below** - Mobile Portrait (compact navbar, scrollable subnav)
- **360px and below** - Small Mobile (ultra-compact, hidden non-essentials)
- **Landscape Mode** - Special optimizations for horizontal orientation

### Mobile Optimizations
- ✅ Collapsible navigation elements
- ✅ Horizontal scrolling subnav
- ✅ Touch-friendly button sizes
- ✅ Optimized image sizes
- ✅ Single column card layout
- ✅ Stacked footer sections
- ✅ Reduced font sizes for readability

## 🔮 Future Enhancements

- [ ] JavaScript interactivity (dropdown menus, modals)
- [ ] Product carousel/slider with autoplay
- [ ] Dynamic search functionality
- [ ] Shopping cart state management
- [ ] User authentication flow
- [ ] Dark mode toggle
- [ ] Product detail pages
- [ ] Backend API integration
- [ ] ARIA labels for accessibility
- [ ] Performance optimization (lazy loading)

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Contribution Guidelines
- Follow existing code style and formatting
- Add comments for complex CSS logic
- Test across multiple browsers and devices
- Update documentation as needed
- Write clear, descriptive commit messages

## 📄 License

This project is licensed under the MIT License.

**MIT License Summary:**
- ✅ Commercial use
- ✅ Modification
- ✅ Distribution
- ✅ Private use

## 🙏 Acknowledgments

- **Design Inspiration**: Amazon.com
- **Fonts**: [Google Fonts - Roboto](https://fonts.google.com/specimen/Roboto)
- **Deployment**: [Vercel](https://vercel.com)
- **Learning Resources**: MDN Web Docs, CSS-Tricks, W3Schools

---

**Made with ❤️ and CSS Grid**

*This project is created for educational purposes and is not affiliated with Amazon.com*

**Live Demo**: [https://amazon-clone-one-coral.vercel.app](https://amazon-clone-one-coral.vercel.app)