# TailwindCSS-NinjaFood

https://tailwindcss.com/docs/installation

**Font Size**: https://tailwindcss.com/docs/font-size#app
**Customizing Colors**: https://tailwindcss.com/docs/customizing-colors#app
**Icons**: https://heroicons.dev/

Give credit to Net Ninja for my learning here: https://www.youtube.com/playlist?list=PL4cUxeGkcC9gpXORlEHjc5bgnIi5HEGhw
Many Thanks to Net Ninja!

Source code references: https://github.com/iamshaunjp/tailwind-tutorial/tree/lesson-1

Using Live-server (development server) to run the website in this project:

1. Install live-server globally
   To install it globally, run: npm install -g live-server
   This will make the live-server command available globally on your machine: **live-server public**

2. Run live-server locally (without global installation)
   Alternatively, you can run live-server from the locally installed node module by using npx: **npx live-server public**

# Notice:

for those who are following this tutorial in 2024 with the latest tailwindcss version:
(from @Jacksons_are_jackson - youtube comment)

1: npx tailwindcss init --full (with default configuration displayed) or without "full" to get the blank config file

2: update tailwind.config.js file according to the following
<code>
/\*_ @type {import('tailwindcss').Config} _/
module.exports = {
content: [
"./public/index.html" -- replace this with your path to your html file
]
...
}
</code>

3. npx tailwindcss -i ./src/styles.css -o ./public/styles.css --watch
   (update this command in package.json for script to run tailwindcss)
