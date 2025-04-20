# Food Reviews by On The Ground YouTubers 🌎🍽️

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Netlify Status](https://api.netlify.com/api/v1/badges/xxxxx-xxxxx-xxxxx/deploy-status)](https://app.netlify.com/)

A curated directory of authentic food reviews from local YouTubers around the world. Find your next dining destination through the eyes of content creators who know their local food scene best.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Getting Started](#getting-started)
- [Directory Structure](#directory-structure)
- [Customization Guide](#customization-guide)
- [Deployment](#deployment)
- [Custom Domain Setup](#custom-domain-setup)
- [Troubleshooting](#troubleshooting)
- [Resources](#resources)
- [Contributing](#contributing)
- [License](#license)

## Overview

This directory website showcases food reviews from YouTubers worldwide, organized in a responsive 3-column grid layout. Each entry features:
- YouTuber profile
- Restaurant information
- Video review link
- Location data
- Cuisine type
- Price range

## Features

- 🔍 Advanced search functionality
- 📱 Responsive design
- 🏷️ Category filtering
- 🗺️ Location-based sorting
- 💰 Price range filters
- 🎥 Direct YouTube video embedding
- 📍 Interactive map integration

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- Git

### Installation

```bash
# Clone the repository
git clone https://github.com/yourusername/food-reviews-directory.git

# Navigate to project directory
cd food-reviews-directory

# Install dependencies
npm install

# Start development server
npm run dev
```

## Directory Structure

```
food-reviews-directory/
├── src/
│   ├── components/
│   ├── data/
│   ├── styles/
│   └── utils/
├── public/
│   ├── images/
│   └── icons/
├── config/
└── package.json
```

## Customization Guide

### Adding New Directory Items

1. Navigate to `src/data/reviews.js`
2. Add new entry following this format:

```javascript
{
  id: "unique-id",
  youtuber: "Channel Name",
  restaurant: "Restaurant Name",
  location: "City, Country",
  cuisine: "Cuisine Type",
  priceRange: "$$$",
  videoUrl: "https://youtube.com/watch?v=xxxxx",
  coordinates: {
    lat: 00.000000,
    lng: 00.000000
  }
}
```

### Modifying Category Labels

Edit `src/data/categories.js`:

```javascript
export const categories = [
  "Street Food",
  "Fine Dining",
  "Hidden Gems",
  "Local Favorites"
];
```

### Updating Hero Section

1. Open `src/components/Hero.js`
2. Modify content within the component:

```javascript
<HeroContainer>
  <HeroTitle>Your New Title</HeroTitle>
  <HeroSubtitle>Your New Subtitle</HeroSubtitle>
</HeroContainer>
```

### Customizing Colors

Edit `src/styles/theme.js`:

```javascript
export const theme = {
  primary: '#your-color-code',
  secondary: '#your-color-code',
  accent: '#your-color-code'
}
```

## Deployment

### Netlify Deployment

1. Connect your GitHub repository to Netlify
2. Configure build settings:
   - Build command: `npm run build`
   - Publish directory: `dist`
3. Click "Deploy"

### Vercel Deployment

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel
```

## Custom Domain Setup

1. Purchase domain from preferred registrar
2. Add domain in deployment platform
3. Configure DNS settings:
   ```
   A     @     76.76.21.21
   CNAME www   your-site.netlify.app
   ```
4. Wait for DNS propagation (24-48 hours)

## Troubleshooting

### Common Issues

1. **Build Failures**
   ```bash
   npm run build --verbose
   ```

2. **Missing Dependencies**
   ```bash
   npm install --force
   ```

3. **API Connection Issues**
   - Check API keys in `.env`
   - Verify network connectivity
   - Confirm CORS settings

## Resources

- [Documentation](https://docs.example.com)
- [Video Tutorials](https://youtube.com/playlist)
- [Support Forum](https://forum.example.com)
- [API Reference](https://api.example.com)

## Contributing

1. Fork the repository
2. Create feature branch
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. Commit changes
   ```bash
   git commit -m 'Add AmazingFeature'
   ```
4. Push to branch
   ```bash
   git push origin feature/AmazingFeature
   ```
5. Open Pull Request

## License

Distributed under the MIT License. See `LICENSE` for more information.

---

Made with ❤️ by [Your Name](https://github.com/yourusername)

For support, email support@example.com or join our [Discord community](https://discord.gg/example).