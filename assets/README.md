# Public Assets Folder

This folder contains all static assets that will be served directly by the web server.

## Structure

```
public/
└── assets/
    ├── images/
    │   ├── hero/          (Hero section images)
    │   ├── customers/     (Customer section scrolling images)
    │   ├── projects/      (Project showcase images)
    │   └── about/         (About section images)
    └── fonts/             (Font files)
```

## Important Notes

1. **All images should be placed in `public/assets/images/` folder**
2. Files in the `public` folder are served at the root URL path
3. For example: `public/assets/images/hero/heroImg1.jpg` is accessible at `/assets/images/hero/heroImg1.jpg`
4. The `AllAssets.js` file uses `window.location.origin` to create absolute URLs
5. Images are referenced using the exported constants from `src/assets/AllAssets.js`

## Image Naming Convention

- Hero: `heroImg1.jpg`
- Customers: `customerImg1.jpg`, `customerImg2.jpg`, etc.
- Projects: `projectImg1.jpg`, `projectImg2.jpg`, etc.
- About: `aboutImg1.jpg`, `aboutImg2.jpg`, etc.

## Usage Example

```javascript
// In any component
import { HERO_IMG1, CUSTOMER_IMG1, PROJECT_IMG1 } from '../assets/AllAssets';

// Use in JSX
<img src={HERO_IMG1} alt="Hero image" />
```








