# Astro Starter Template ✨

Initial setup for Astro projects with React, Tailwind CSS, Prettier, and automatic import/class sorting.

[![Astro](https://img.shields.io/badge/Astro-5-BC52EE?style=flat-square&logo=astro&logoColor=white)](https://astro.build/)
[![React](https://img.shields.io/badge/React-19-61DAFB?style=flat-square&logo=react&logoColor=black)](https://react.dev/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-4-38bdf8?style=flat-square&logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Prettier](https://img.shields.io/badge/Prettier-3-F7B93E?style=flat-square&logo=prettier&logoColor=black)](https://prettier.io/)

---

## ✨ Features

🚀 **Astro 5** — Fast, content-focused framework  
⚛️ **React 19** — Interactive components with Islands Architecture  
🎨 **Tailwind CSS 4** — Modern styling with dark mode support  
✨ **Prettier** — Consistent formatting with Astro and Tailwind plugins  
🔄 **Auto-sorting** — Imports and classes organized automatically  
📦 **Lucide Icons** — Beautiful, customizable icons  
🗺️ **Sitemap** — Auto-generated sitemap for SEO

---

## 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/vctorgriggi/astro-starter-template.git
cd astro-starter-template

# Install dependencies
npm install

# Run the project
npm run dev
```

Open [http://localhost:4321](http://localhost:4321) 🎉

---

## 🏗️ Project Structure

```
├── public/                   # Static assets
│   ├── favicon.svg          # Site favicon
│   └── site.webmanifest     # Web app manifest
├── src/
│   ├── components/          # Reusable components
│   │   └── layout/          # Layout components (Head, Favicons)
│   ├── data/                # Site constants and config
│   │   └── consts.ts        # Site metadata
│   ├── layouts/             # Page layouts
│   │   └── Layout.astro     # Root layout
│   ├── pages/               # File-based routing
│   │   └── index.astro      # Home page
│   ├── styles/              # Global styles
│   │   └── global.css       # Tailwind + theme variables
│   └── types.ts             # TypeScript types
├── .prettierrc              # Prettier configuration
├── astro.config.mjs         # Astro configuration
└── tsconfig.json            # TypeScript configuration
```

---

## 🛠️ Tech Stack

**Framework** → [Astro 5](https://astro.build/)  
**UI Library** → [React 19](https://react.dev/)  
**Styling** → [Tailwind CSS 4](https://tailwindcss.com/)  
**Formatting** → [Prettier](https://prettier.io/) + [prettier-plugin-astro](https://github.com/withastro/prettier-plugin-astro) + [prettier-plugin-tailwindcss](https://github.com/tailwindlabs/prettier-plugin-tailwindcss)  
**Icons** → [Lucide React](https://lucide.dev/) + [astro-icon](https://github.com/natemoo-re/astro-icon)  
**Font** → [Inter](https://rsms.me/inter/) via Google Fonts  
**Language** → [TypeScript](https://www.typescriptlang.org/)

---

## ⚙️ Configuration

### Prettier

```json
{
  "semi": true,
  "singleQuote": true,
  "tabWidth": 2,
  "plugins": [
    "prettier-plugin-astro",
    "prettier-plugin-tailwindcss",
    "prettier-plugin-astro-organize-imports"
  ]
}
```

Automatically sorts imports and Tailwind classes for consistent code. Note: `prettier-plugin-astro-organize-imports` must be the last plugin in the list.

### TypeScript

Path aliases configured for clean imports:

```json
{
  "compilerOptions": {
    "baseUrl": ".",
    "paths": {
      "@/*": ["./src/*"]
    }
  }
}
```

### Theming

Light and dark mode with CSS variables in `global.css`:

```css
@theme {
  --color-primary: #00a2dd;
  --color-bg: #ffffff;
  --color-text-primary: #0f172a;
}

.dark {
  --color-bg: #0b1220;
  --color-text-primary: #e5e7eb;
}
```

---

## 📜 Scripts

```bash
# Development
npm run dev

# Production build
npm run build

# Preview production build
npm run preview

# Formatting
npm run prettier
```

---

## 🎨 Auto-sorting

### Imports

Sorted automatically via `prettier-plugin-astro-organize-imports`:

1. External libraries (Astro, React)
2. Internal aliases (`@/`)
3. Relative imports
4. CSS and assets

### Tailwind Classes

Sorted automatically via `prettier-plugin-tailwindcss` when running `npm run prettier`.

---

## 🔧 Customization

### Site Metadata

Edit `src/data/consts.ts`:

```ts
export const SITE: Site = {
  title: 'My Astro App',
  description: 'An awesome app built with Astro.',
  href: 'https://myapp.example.com',
  author: 'My Company',
  locale: 'en-US',
};
```

### Prettier Config

Edit `.prettierrc` to adjust formatting preferences.

### Astro Config

Edit `astro.config.mjs` to add integrations or modify settings.

---

## 🤝 Contributing

Contributions are welcome! Open an issue or submit a PR.

---

**[Issues](https://github.com/vctorgriggi/astro-starter-template/issues)**

Made with ❤️ by [vctorgriggi](https://github.com/vctorgriggi)
