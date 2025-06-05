# 🌟 Software Engineer Portfolio Website

A modern, responsive portfolio website built with **Astro** and **Tailwind CSS**, designed for software engineers seeking new opportunities. Features a beautiful glassmorphism design with soft pink pastels and smooth animations.

![Portfolio Preview](https://via.placeholder.com/800x400/f8bbd9/ffffff?text=Portfolio+Website+Preview)

## 🚀 Live Demo

[View Live Portfolio](https://your-portfolio-url.com) *(Replace with your actual deployment URL)*

## ✨ Features

### 🎨 **Modern Design**
- **Glassmorphism UI** with backdrop blur effects
- **Soft Pink Gradient** color scheme throughout
- **Smooth Animations** and hover effects
- **Professional Typography** with proper hierarchy
- **Responsive Design** that works on all devices

### 🧩 **Modular Component Architecture**
- **Reusable Components** for easy maintenance
- **TypeScript Support** for better development experience
- **Clean Code Structure** following best practices
- **Easy Customization** through component props

### 📱 **Mobile-First Responsive**
- **Touch-Friendly** interface with proper tap targets
- **Adaptive Layouts** for mobile, tablet, and desktop
- **Optimized Typography** scaling across screen sizes
- **No Horizontal Scrolling** on any device

### 🏢 **Professional Sections**
- **Hero Section** with personal branding
- **Work Experience** with detailed job history
- **Skills & Technologies** organized by category
- **Social Links** with hover animations
- **Availability Status** indicator

## 🛠️ Tech Stack

- **[Astro 5.8.2](https://astro.build)** - Static Site Generator
- **[Tailwind CSS 4.1.8](https://tailwindcss.com)** - Utility-First CSS Framework
- **[TypeScript](https://www.typescriptlang.org)** - Type Safety
- **[Prettier](https://prettier.io)** - Code Formatting

## 📂 Project Structure

```
fumbling-filament/
├── src/
│   ├── components/           # Reusable UI components
│   │   ├── Avatar.astro     # Profile picture placeholder
│   │   ├── CTAButtons.astro # Call-to-action buttons
│   │   ├── ExperienceCard.astro # Individual job experience
│   │   ├── ExperienceSection.astro # Complete work history
│   │   ├── HeroSection.astro # Main hero area
│   │   ├── SkillCard.astro  # Individual skill category
│   │   ├── SkillsSection.astro # Technologies & skills
│   │   ├── SocialLinks.astro # Social media icons
│   │   ├── StatusIndicator.astro # Availability status
│   │   └── Welcome.astro    # Main page component
│   ├── layouts/
│   │   └── Layout.astro     # Base HTML layout
│   ├── pages/
│   │   └── index.astro      # Homepage
│   ├── styles/
│   │   └── global.css       # Global styles
│   └── assets/              # Static assets
├── public/                  # Public assets
├── package.json
├── astro.config.mjs
├── tailwind.config.js
└── README.md
```

## 🚀 Getting Started

### Prerequisites

- **Node.js 18+** or **Bun**
- **Git**

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/portfolio-website.git
   cd portfolio-website
   ```

2. **Install dependencies**
   ```bash
   # Using npm
   npm install
   
   # Using yarn
   yarn install
   
   # Using bun
   bun install
   ```

3. **Start development server**
   ```bash
   # Using npm
   npm run dev
   
   # Using yarn
   yarn dev
   
   # Using bun
   bun run dev
   ```

4. **Open in browser**
   ```
   http://localhost:4321
   ```

## 🎨 Customization Guide

### 📝 **Personal Information**

Edit `src/components/HeroSection.astro`:

```astro
<h1>Your Name Here</h1>
<h2>Your Job Title</h2>
<p>Your bio description...</p>
```

### 🏢 **Work Experience**

Edit `src/components/ExperienceSection.astro`:

```javascript
const experiences = [
  {
    company: "Your Company",
    position: "Your Position",
    duration: "2022 - Present",
    description: "Your job description with achievements...",
    technologies: ["React", "Node.js", "AWS"],
    isCurrentJob: true
  },
  // Add more experiences...
];
```

### 💻 **Skills & Technologies**

Edit `src/components/SkillsSection.astro`:

```javascript
const skillCategories = [
  {
    title: "Frontend",
    skills: ["React", "Vue.js", "TypeScript"]
  },
  {
    title: "Backend", 
    skills: ["Node.js", "Python", "PostgreSQL"]
  },
  // Add more categories...
];
```

### 🔗 **Social Links**

Edit `src/components/SocialLinks.astro`:

```astro
<a href="https://github.com/yourusername">GitHub</a>
<a href="https://linkedin.com/in/yourprofile">LinkedIn</a>
<a href="mailto:your.email@example.com">Email</a>
```

### 🖼️ **Profile Picture**

Replace the placeholder in `src/components/Avatar.astro` with your actual photo:

```astro
<img src="/your-photo.jpg" alt="Your Name" class="w-30 h-30 rounded-full" />
```

## 🎨 Design System

### 🌈 **Color Palette**

```css
/* Primary Pink Gradient */
from-pink-300 to-pink-500  /* #f8bbd9 to #e879b9 */

/* Background Colors */
bg-white/80               /* Semi-transparent white */
bg-gray-100              /* Light gray backgrounds */

/* Text Colors */
text-gray-900            /* Primary text */
text-gray-600            /* Secondary text */
text-pink-500            /* Accent text */
```

### 📱 **Responsive Breakpoints**

```css
/* Mobile First Approach */
sm: 640px     /* Small devices */
md: 768px     /* Medium devices */
lg: 1024px    /* Large devices */
xl: 1280px    /* Extra large devices */
```

### ✨ **Animation Classes**

```css
/* Hover Effects */
hover:-translate-y-1     /* Lift on hover */
hover:scale-105         /* Scale on hover */
transition-all duration-300  /* Smooth transitions */

/* Loading States */
animate-pulse           /* Pulsing animation */
animate-ping           /* Ping animation */
```

## 📦 Build & Deployment

### 🏗️ **Build for Production**

```bash
npm run build
```

### 🌐 **Deployment Options**

#### **Vercel** (Recommended)
1. Push to GitHub
2. Connect repository to Vercel
3. Deploy automatically

#### **Netlify**
1. Push to GitHub
2. Connect repository to Netlify
3. Set build command: `npm run build`
4. Set publish directory: `dist`

#### **GitHub Pages**
```bash
npm run build
# Upload dist/ folder to gh-pages branch
```

## 🔧 Scripts

```bash
npm run dev      # Start development server
npm run build    # Build for production
npm run preview  # Preview production build
```

## 📊 Performance Features

- **⚡ Fast Loading** - Optimized with Astro's static generation
- **📱 Mobile Optimized** - Responsive design with touch-friendly interface
- **🎨 Smooth Animations** - Hardware-accelerated CSS animations
- **♿ Accessible** - Proper ARIA labels and semantic HTML
- **🔍 SEO Ready** - Meta tags and structured data support

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **[Astro Team](https://astro.build)** for the amazing static site generator
- **[Tailwind CSS](https://tailwindcss.com)** for the utility-first CSS framework
- **Design Inspiration** from modern portfolio websites and glassmorphism trends

## 📞 Support

If you have any questions or need help customizing your portfolio:

- 📧 **Email**: your.email@example.com
- 🐦 **Twitter**: [@yourusername](https://twitter.com/yourusername)
- 💼 **LinkedIn**: [Your Profile](https://linkedin.com/in/yourprofile)

---

**⭐ Star this repository if it helped you create an amazing portfolio!**

Made with ❤️ and modern web technologies