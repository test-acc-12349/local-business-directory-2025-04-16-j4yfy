# Local Business Directory

> Discover the best local businesses in one place - A comprehensive directory website featuring a modern 3-column grid layout.

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Directory Structure](#directory-structure)
- [Customization](#customization)
  - [Directory Items](#directory-items)
  - [Categories](#categories)
  - [Hero Section](#hero-section)
  - [Styling](#styling)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Resources](#resources)
- [Support](#support)

## Overview

Local Business Directory is a responsive directory website that helps users discover and connect with local businesses. The website features a clean, modern design with a 3-column grid layout, category filtering, and search functionality.

## Features

- Responsive 3-column grid layout
- Category-based filtering
- Search functionality
- Business detail pages
- Contact forms
- Social media integration
- Mobile-friendly design
- SEO optimized
- Fast loading times

## Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- Basic knowledge of HTML/CSS
- Text editor (VS Code recommended)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/local-business-directory.git
```

2. Install dependencies:
```bash
cd local-business-directory
npm install
```

3. Start the development server:
```bash
npm run dev
```

## Directory Structure

```
local-business-directory/
├── src/
│   ├── components/
│   ├── data/
│   ├── styles/
│   └── pages/
├── public/
│   └── images/
├── package.json
└── README.md
```

## Customization

### Directory Items

Add or edit directory items in `src/data/directory.js`:

```javascript
export const directoryItems = [
  {
    id: "1",
    name: "Business Name",
    category: "Category",
    description: "Business description",
    address: "Business address",
    phone: "Phone number",
    website: "Website URL",
    image: "/images/business.jpg"
  }
];
```

### Categories

Modify categories in `src/data/categories.js`:

```javascript
export const categories = [
  "Restaurants",
  "Retail",
  "Services",
  "Entertainment"
];
```

### Hero Section

Update the hero section in `src/components/Hero.js`:

```javascript
const heroContent = {
  title: "Your Title",
  subtitle: "Your Subtitle",
  backgroundImage: "/images/hero-bg.jpg"
};
```

### Styling

Customize colors and styles in `src/styles/variables.css`:

```css
:root {
  --primary-color: #007bff;
  --secondary-color: #6c757d;
  --background-color: #ffffff;
  --text-color: #333333;
}
```

## Deployment

1. Build the project:
```bash
npm run build
```

2. Deploy to your preferred hosting platform:
- Vercel
- Netlify
- GitHub Pages

## Custom Domain Setup

1. Purchase a domain from a registrar
2. Add DNS records:
```
A     @     76.76.21.21
CNAME www   yourdomain.com
```

3. Configure domain in hosting platform settings
4. Wait for DNS propagation (24-48 hours)

## Troubleshooting

Common issues and solutions:

- **Images not loading**: Ensure correct path in public directory
- **Styling issues**: Clear browser cache and rebuild
- **Build errors**: Check console for specific error messages
- **Category filter not working**: Verify category names match exactly

## Resources

- [Documentation](https://docs.yourdomain.com)
- [API Reference](https://api.yourdomain.com)
- [Style Guide](https://style.yourdomain.com)
- [Contributing Guidelines](CONTRIBUTING.md)

## Support

- Create an issue in the GitHub repository
- Email support: support@yourdomain.com
- Join our [Discord community](https://discord.gg/yourdirectory)

---

© 2024 Local Business Directory. Released under the MIT License.