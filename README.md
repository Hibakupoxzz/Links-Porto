# Astro Links Website - Dark Theme with Purple Icons 💜

Simple personal links website built with Astro.js featuring flat dark background and purple icons.

## 🚀 Project Structure

```
/
├── public/
│   └── (place your images here, e.g., profile.jpg)
├── src/
│   ├── components/
│   │   ├── LinkCard.astro      # Individual link card component
│   │   └── LinkSection.astro    # Section wrapper component
│   ├── layouts/
│   │   └── Layout.astro         # Base layout with styles
│   └── pages/
│       └── index.astro          # Main page
├── astro.config.mjs
├── package.json
└── tsconfig.json
```

## 🎨 Color Scheme

- **Background:** `#0f0f0f` (flat dark gray/black)
- **Icons:** `#a78bfa` (purple)
- **Icon Hover:** `#c4b5fd` (lighter purple)
- **Accent Text:** Purple gradient
- **Border:** `#2a2a2a` (dark gray)
- **Hover Effect:** Purple glow with `#8b5cf6`

## 📦 Installation

1. Install dependencies:
```bash
npm install
```

2. Start development server:
```bash
npm run dev
```

3. Build for production:
```bash
npm run build
```

4. Preview production build:
```bash
npm run preview
```

The dev server will run on `http://localhost:4321`

## ✏️ Customization

### Add Your Profile Image

1. Place your image in the `public/` folder (e.g., `public/profile.jpg`)
2. In `src/pages/index.astro`, uncomment and update:
```astro
<img src="/profile.jpg" alt="Profile" />
```

### Update Your Name

In `src/pages/index.astro`, change:
```astro
<h1>Your<span class="highlight">Name</span></h1>
```

### Update Links

Edit the `LinkCard` components in `src/pages/index.astro`:
```astro
<LinkCard name="Your Link Name" url="https://your-url.com" icon={iconVariable} />
```

### Add/Remove Sections

Use the `LinkSection` component:
```astro
<LinkSection title="Section Name" icon={iconSVG}>
  <LinkCard name="Link 1" url="#" icon={icon1} />
  <LinkCard name="Link 2" url="#" icon={icon2} />
</LinkSection>
```

### Add New Icons

Add icon SVG paths at the top of `src/pages/index.astro`:
```astro
const myIcon = `
  <path d="...your SVG path..."/>
`;
```

## 🎯 Features

- ✅ Flat dark background (#0f0f0f)
- ✅ All icons in purple (#a78bfa)
- ✅ Official Itch.io logo
- ✅ Purple gradient title effect
- ✅ Smooth hover animations
- ✅ Purple glow effects
- ✅ Glassmorphism on cards
- ✅ Component-based architecture
- ✅ Fully responsive
- ✅ Fast performance with Astro

## 📱 Responsive

Fully responsive design that works on:
- Desktop (768px+)
- Tablet (640px - 768px)
- Mobile (< 640px)

## 🔧 Tech Stack

- [Astro](https://astro.build) - Static site generator
- Pure CSS (no frameworks)
- SVG icons (including official Itch.io logo)

## 📚 Icon Sources

- **Lucide Icons:** https://lucide.dev (Twitter, Discord, Reddit, LinkedIn, GitHub, etc.)
- **Itch.io Logo:** Official Itch.io Press Kit (https://itch.io/press-kit)

## 📝 Notes

- All icons are colored purple (#a78bfa) by default
- Hover effect changes icon to lighter purple (#c4b5fd)
- Background is flat solid color for clean look
- Profile image has purple glow effect

## 📄 License

Free to use for personal projects!
