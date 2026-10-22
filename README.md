# SKDev — Digital Portfolio

A React portfolio for SKDev that presents Android apps, experiments, and ways to get in touch. The desktop experience features interactive 3D scenes and motion; the layout also adapts to smaller screens and reduced-motion preferences.

Live site: https://skdev.psatyakiran.in

## What’s inside

- An animated opening sequence, custom pointer effects, page transitions, and optional interface sounds.
- A mouse-interactive 3D phone demo for Anify, Milky Launcher, and Aniset. Visitors can switch apps, explore sample screens, and follow links to Google Play.
- Selected-work cards and individual app pages with screenshots, details, and download links.
- A playable 3D Snake game, plus interactive roadmap and progress sections.
- Roadmap, freelance/contact, FAQ, support, and privacy pages.
- Installable PWA support, search and social metadata, and generated route metadata for sharing.

## Tech stack

- React 19 and Vite 8
- React Router
- Three.js
- Lucide icons
- vite-plugin-pwa

## Run the project

Requirements: Node.js 24.x and npm.

    npm install
    npm run dev

Vite prints the local address in the terminal. Open that address in a browser.

## Useful commands

    npm run dev       Start the development server
    npm test          Run the Snake game logic tests
    npm run lint       Check the source with ESLint
    npm run build      Create a production build and route metadata
    npm run preview    Preview the production build locally

The production files are written to the dist directory.

## Project map

    public/                 Static files, icons, manifest, and site metadata
    scripts/                Build helpers, including route metadata generation
    src/assets/             App artwork, screenshots, and brand images
    src/components/         Shared navigation, footer, SEO, and UI components
    src/data/appsData.js    App descriptions, screenshots, and store links
    src/experience/         3D phone, Snake game, transitions, sound, and motion
    src/pages/              Home, app, roadmap, FAQ, support, and contact pages
    src/App.jsx              App routes and shared page layout
    vite.config.js           Vite and PWA configuration
    vercel.json              SPA route fallback for Vercel

## Main routes

- / — portfolio home and interactive playground
- /apps — app collection
- /apps/:id — app details
- /roadmap — development roadmap
- /freelance — services and contact
- /faq — frequently asked questions
- /donate — support options
- /privacy — privacy policy

## Update app information

Edit src/data/appsData.js to update app names, descriptions, screenshots, compatibility details, and store links. Put imported artwork in src/assets/. Static files such as the web manifest and icons belong in public/.

## Publish from the source ZIP to GitHub

Create an empty GitHub repository. Extract the ZIP, open a terminal in the extracted skdev-website folder, and replace the example URL below with your repository URL:

    git init
    git add .
    git commit -m "Add SKDev website"
    git branch -M main
    git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
    git push -u origin main

For Vercel, import the Git repository and use npm run build as the build command with dist as the output directory. The included Vercel configuration routes app pages back to the single-page app.

## Credits

The portfolio presents the work of Satyakiran / SKDev. The interactive website experience is credited to Arman at [sandhiarman185@gmail.com](mailto:sandhiarman185@gmail.com) and [@Arman_0G](https://t.me/Arman_0G), with GPT 6 Luna assistance.

