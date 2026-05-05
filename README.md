# Resources Bento Stack

A beautiful, curated bento-grid showcase for your favorite online resources.

## 🚀 How to Customize

All the data for this website is stored in `src/constants.ts`. You don't need to touch the main logic to add your links!

### 1. Change Site Identity
Find the `SITE_CONFIG` object at the bottom of `src/constants.ts`:
```typescript
export const SITE_CONFIG = {
  name: 'Your Stack Name',
  description: 'A brief description of what you are showcasing.',
  author: 'Your Name'
};
```

### 2. Add a Website
Add a new object to the `RESOURCES` array:
```typescript
{
  id: 'unique-id',
  title: 'Website Name',
  description: 'Fast description of the resource.',
  url: 'https://...',
  iconName: 'Layout', // Use any PascalCase icon name from lucide-react
  size: 'medium',   // options: small, medium, large, wide, tall
  category: 'Design',
  accentColor: '#FF0000' // Hex code for the icon background
}
```

### 3. Icon Selection
We use **Lucide Icons**. You can find all available icon names at [lucide.dev](https://lucide.dev/icons). Just use the PascalCase version (e.g., `HeartPulse` for `heart-pulse`).

---

## 🌍 How to Deploy


### Netlify / Vercel (Manual)
1. Export the code as a ZIP from the Settings menu.
2. Run `npm install` and `npm run build`.
3. Drag the `dist` folder to Netlify or push the code to a GitHub repo and connect it to Vercel/Netlify.
