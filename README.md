# Frameworks CA: Spcial Media App

A simple, responsive social media prototype built with HTML and Tailwind CSS. This project demonstrates how to use a CSS framework (Tailwind) to create a multi-page app with authentication, a feed, and a user profile—all styled without custom media queries.

## 🚀 Features
- Authentication page (index.html)

  - Login/register form with HTML validation

  - Password minimum length enforcement

  - Centered, card-style layout
 
- Feed page (feed/index.html)

  - Search bar & sort dropdown

  - Responsive grid of post cards with thumbnails

  - “New post” floating action button
 
- Profile page (profile/index.html)

  - Profile avatar, username, follower/following counts

  - Follow button

  - Grid of user’s posts
 
- Responsive design

  - Mobile-first approach

  - Breakpoints at sm/md/lg/xl (Tailwind defaults)
 
- Build setup

  - Tailwind CSS (v3+) via PostCSS

  - npm run dev for development watch

  - npm run build for production CSS
 
## 📂 Project structure
```bash
.
├── index.html           # Authentication page
├── feed/
│   └── index.html       # Feed page
├── profile/
│   └── index.html       # Profile page
├── css/
│   └── style.css        # Compiled Tailwind output
├── src/
│   └── styles.css       # Tailwind directives & custom base styles
├── tailwind.config.js   # Tailwind content/theme config
├── postcss.config.js    # PostCSS + Autoprefixer config
├── package.json         # Scripts & dependencies
└── README.md
```

## ⚙️ Setup & Development

1. Clone this repository and switch to the css-frameworks branch:
 ```bash
git clone https://github.com/AilinMari/framework-ca.git
cd framework-ca
git checkout css-frameworks
```
2. Install dependencies:
   ```bash
   npm install

3. Build Tailwind CSS and watch for changes (development):
```bash
npm run dev
```
- Edits to src/styles.css or any HTML file under index.html, feed/, or profile/ will trigger an automatic rebuild of css/style.css.
4. Production build:
  ```bash
  npm run build
```
- Outputs a minified css/style.css ready for deployment.

5. Serve the files (using any static-server):
```bash
npx serve .
```
- Open http://localhost:5000/index.html to view the login page, then navigate to feed/index.html and profile/index.html.

  ## 🛠️ Scripts
| Command         | Description                                  |
| --------------- | -------------------------------------------- |
| `npm run dev`   | Build & watch Tailwind CSS for changes       |
| `npm run build` | Generate a production-ready CSS file         |
| *(Optional)*    | Use any static-server to serve `.` directory |

## 📚 Learnings
- How to integrate Tailwind CSS via PostCSS (no CDN)

- Building mobile-first, responsive layouts with utility classes

- Organizing multiple pages in a statically served app

- Managing NPM scripts for development vs. production

 ## 👩‍🎓 Author
Ailin-Mari Bøe<br>
Course Assignment: CSS Frameworks CA
##
Feel free to explore, tweak the design, and reuse this setup for your own Tailwind-powered projects!
