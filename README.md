# Assignment10-Jo-DIkta-Hai_Wo-Bikta-Hai
## Theory

Qn1.Explore all the ways of writing CSS?
- 1. By using external files.eg. index.css
- 2. By using Inline CSS
- 3. By using styled components- (https://styled-components.com/)
- 4. SCSS or CSS
- 5. By using libraries like- 
- MAterial UI- (https://mui.com/),
- CHakra UI-(https://chakra-ui.com/) etc

Qn2.How do we configure Tailwind?

- Configuring TAilwind by-
- 1. Via CDN
- Include this script tag in html -
- ###   <script src="https://cdn.tailwindcss.com"></script>

- 2. Via Npm package
- 1. Install tailwind and it's dependency- postcss also.
- ### npm install -D tailwindcss postcss autoprefixer
- ### npx tailwindcss init

- 2. COnfigure tailwind.config.js file
- module.exports = {
-  content: ["./src/**/*.{html,js}"],
-  theme: {
-   extend: {},
- },
- plugins: [],
- }

- 3. Create a file named .postcssrc & Configure it.
- module.exports = {
-  plugins: {
-    tailwindcss: {}
- }
- }

- 4. Inside index.css file 📝
- @tailwind base;
- @tailwind components;
- @tailwind utilities;

Qn3.IN tailwind.config.js, what does all the keys mean(content,theme,extend,plugins)?

- 1. CONTENT- The content section of your tailwind.config.js file is where you configure the paths to all of your HTML templates, JavaScript components, and any other source files that contain Tailwind class names.
- 2. THEME-The theme section of your tailwind.config.js file is where you define your project’s color palette, type scale, fonts, breakpoints, border radius values, and more.
- 3. EXTEND- If you’d like to preserve the default values for a theme option but also add new values, add your extensions under the extend key in the theme section of your configuration file.
- 4. PLUGINS- Plugins let you register new styles for Tailwind to inject into the user’s stylesheet using JavaScript instead of CSS.

Qn4.WHy do we have .postcssrc file?

- We have .postcssrc for the configuration of postcss 
- It tells our bundler that while you are bundling things up, we will be using tailwind for css.SO. compile tailwind to normal css.