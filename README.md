# TailwindCSS-NinjaFood

https://tailwindcss.com/docs/installation

**Font Size**: https://tailwindcss.com/docs/font-size#app
**Customizing Colors**: https://tailwindcss.com/docs/customizing-colors#app

Give credit to Net Ninja for my learning here: https://www.youtube.com/playlist?list=PL4cUxeGkcC9gpXORlEHjc5bgnIi5HEGhw
Many Thanks to Net Ninja!

Source code references: https://github.com/iamshaunjp/tailwind-tutorial/tree/lesson-1

Using Live-server (development server) to run the website in this project:

1. Install live-server globally
   To install it globally, run: npm install -g live-server
   This will make the live-server command available globally on your machine: **live-server public --no-css-inject**

2. Run live-server locally (without global installation)
   Alternatively, you can run live-server from the locally installed node module by using npx: **npx live-server public --no-css-inject**

   Why added "--no-css-inject"?
   -->
   <code>
   If anyone finds they have to save the file twice to see changes, it'd be because the Live-Server picks up the HTML changes before tailwind has finished building the CSS file and doesn't register the change
   Instead of > live-server public
   Try > live-server public --no-css-inject
   This will update the page again when the tailwindcss finishes building so you don't have to refresh twice.
   (from @shaunrussell1020 - youtube comment)
   </code>

# Notice:

for those who are following this tutorial in 2024 with the latest tailwindcss version:
(from @Jacksons_are_jackson - youtube comment)

1: npx tailwindcss init

2: update tailwind.config.js file according to the following
<code>
/\*_ @type {import('tailwindcss').Config} _/
module.exports = {
content: [
"./public/index.html" -- replace this with your path to your html file
]

      ,
      theme: {
      extend: {},
      },
      plugins: [],
      };
      </code>

3. npx tailwindcss -i ./src/styles.css -o ./public/styles.css --watch
   (update this command in package.json for script to run tailwindcss)
