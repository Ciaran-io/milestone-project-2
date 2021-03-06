# Explore Ireland

![Explore Ireland](./src/assets/images/explore-ireland-screen-shot.png)

This web application was built as part of my projects for Code Institute full-stack web development. The single-page application provides users with locations throughout Ireland that are interested in popular tourist destinations, cycling trail destinations & walking trails destinations. The user is provided with the locations through google maps and accessible links.

---

### <u>Table of contents</u>

<details>
<summary>Table of contents</summary>

1. [Technologies used](#technologies)

   - [Frameworks](#frameworks)
   - [API's](#apis)
   - [Tools](#Tools)
   - [Additional Build Tools](#additional-build-tools)

2. [Features](#features)

   - [Features](#features)
   - [Future Features](#future-features)

3. [Design UX/UI](design-ux/ui)

   - [UX](#ux)
   - [UI](#ui)

4. [Testing](#testing)

   - [Automated Testing](#automated-testing)
   - [Manual Testing](#manual-testing)

5. [Deployment](#deployment)

   - [How To Run The Project Locally](#how-to-run-the-project-locally)
   - [How To Build Project Before Deployment](#how-to-build-the-project-before-deployment)

6. [Credits](#credits)

   - [Contents](#contents)
   - [Media](#media)
   - [Code contribution](#code-contribution)
   - [Acknowledgments](#acknowledgments)

</details>

---

## Technologies

- Languages: HTML, CSS & Javascript.
- Frameworks: TailwindCSS
- API's : Goolge Maps, EmailJS, Google Fonts

### Frameworks

- [Tailwindcss](https://tailwindcss.com/)
  > Tailwindcss is a utility first CSS framework where you use HTML class to declare your CSS inside the Html file using HTML syntax.

### API's

- Google Maps Javascript API

> Google maps API is used to display the user with the trail locations using map icons using data from the application.

- EmailJs
  > EmailJs is used to send a message to the author using the contact form provided. The form accepts the user's name, message & email & forwards the details to the author.

<br> 
### Tools

- [VScode](https://code.visualstudio.com/): IDE used for code editing.
- [Git](https://git-scm.com/download/mac): Used for version control.
- [Github](https://github.com): Used to store & view the project outside local envoirnemt.
- [Figma](https://www.figma.com/): Used for wireframes & design for the project.
- [Affinity Designer](https://affinity.serif.com/en-us/designer/): Used to make favicon for site.
  <br>

### Additional Build Tools

<p>The following packages were added to the application final build for performance.</P>

- [PostCSS](https://postcss.org/)

> Postcss is a plugin for tailwind that enables future CSS to be used in the project & adds auto prefixes to the final CSS build for older browsers support.

- [CSS nano](https://cssnano.co/)

> CSS nano is a postcss plugin used to minify CSS in the final build process.

- [Terser](https://terser.org)

> Terser is an npm package used to minify javascript files in the final build process.

- [Imagemin webp](https://www.npmjs.com/package/imagemin-webp)

> Imagemin is an npm package used to convert jpeg files to webp files.
> Used for decreasing image file size.

- [PurgeCSS](https://purgecss.com/plugins/postcss.html)
  > Purge CSS is a npm package used to remove unused styles in the HTML document.

---

### Features

- Feature 1 - Allows users to view popular trails around Ireland from a choice of cycling trails, walking trails & popular tourist locations by clicking on the discover now buttons & providing the user with locations on google maps.

- Feature 2 - Provides direct links to google maps for popular tourist destinations throughout Ireland.

- Feature 3 - Allows the user to send a message to the author through a contact form.

###Future Features

- To add search functionality and filtering to allow the user to search based on county, & filter based on activity.

- To add the ability for the user to add their selection to google maps and will show the distance to location from their current position.

---

## Design UX/UI

### UX

Goals:

1. To provide the user with a map of walking trails & cycle trail locations around Ireland as well as popular tourist destinations.
2. To provide the user with the ability to send a message to the author through a contact form.

(1) The goals of the application provide users with popular destinations around Ireland for Cycling trails, walking trails & popular tourist destinations around Ireland. This is achieved both when the user clicks on the discover now buttons which will display the list of locations along with a google map that displays location icons around Ireland. When the user clicks on the map icon a tooltip with the location name and county name will be displayed.

There is also cards displays to the user with a button displayed to show more. When the user click on on any of the cards button it will show the county where the trail is located

(1) There is another section the has direct links in the quickly explore section. This section contains three cards with 3 links in each card. The link will highlight when the user hovers over the link with a mouse or pressing on the link through mobile or tablet. The links send the user to google maps will provide the user with the destination and further details on the selected location.

(2) A contact form provides the user with the ability to contact the author. The user will need to provide a name, message and valid email. All inputs from the user are required. If an input is missed when the user clicks on the send mail button a tooltip will be applied to the input asking the user to input their details along with the input being highlighted.

### UI

- Design: Wireframes, colours, icons & fonts are available to view from the Figma browser app.
  The link below will open Figma in the browser & will display the project. The project has 4 sections that show the projects images, fonts & how the web application will look on mobile, tablet & desktop devices.

 <u>

- [Explore Ireland wireframes & design](https://www.figma.com/file/hkC3QpDgfOhyjbMaIzrfO1/Milestone-Project-2?node-id=0%3A1 'Link to figma')
  </u>

<br>

---

## Testing

### Automated Testing

> The following testing tools where used got my site & check for possible errors and warnings.

- [W3C HTML Markup Validation:](https://validator.w3.org/ 'Link to w3C HTML markup validations') used to validate HTML. Result displayed no errors or warnings.
- [W3C CSS Markup Validation:](https://jigsaw.w3.org/css-validator/ 'Link to w3C CSS markup validations') used to validate CSS. The result displayed 5 errors. The errors are not present before the build process and the css is valid before the build process.
- [Jshint Javascript Markup Validation:](https://jshint.com/ 'Link to Jshint Javascript markup validations') used to validate Javascript. The result displayed 3 errors on the maps.js script.

 <br>
 Javascript Issues: Three warnings in line 214, 226, 237 "The body of a for in should be wrapped in an if statement to filter unwanted properties from the prototype." I had issues with the google map being called based on the user clicking on the discover now button, for now, all the map locations are called when the page is loaded

 <br>

### Manual Testing

> Button Elements:

- Discover now button inside discover now cards.

- Clicked on each button to display the selected information (A list of the locations in cards & google maps with location icons).

- The button text colour will change to highlight which button selected.
- The button will display an outline border colour to emphasize the button pressed or clicked.
- When another discover now button is selected the previous selections will be hidden.
- When the discover now button is re-selected all sections will be hidden.

 <br>

- Find out more button in the map section.

- When a button is selected all cards inside the list will display the county information for there destinations and the card's properties will increase. The button will then show an option for 'show less'. When the show less option is all cards will remove the county information and the cards height properties will be changes.
  <br>

> Google Map icons

- When icons inside the map are clicked a tooltip window will display, the information of the selected icon will display the destination location & county of the destination.
  <br>

> Page Links

- Clicked each link inside the places of interest cards. Verified links work and that they return the correct location as described in the link.
  <br>

> Contact Form Validation

- Check each input is required my manually clicking send an email. A tooltip will display under the input displaying the input is required.
  <br>

> Developer Tools Testing

- Tested mobile and desktop site using lighthouse tools in Google Chrome.
  Note: See results at end of testing documentation. The result is shown in png images.
  <br>

> Issued to resolve:

- Remove render blocking css.
- Defer offscreen images.
  <br>

> Tested Browsers

- Note: on desktop developer tools were used to check for errors in the console & view how the application would view across multiple viewing sizes using the responsive mode in the toggle device toolbar option.
  <br>

> Desktop tested browser applications

- Safari
- Google Chrome
- Firefox
  <br>

> Mobile tested browser applications

- Safari
  No issues detected in functionality across multiple browsers and devices behaved as expected.

> Note: For mobile devices, possibly implement a filter to the list. If more locations are added to the list it would cause the user to scroll through the entire list which may lead to a bad user experience.

> Lighthouse testing results.

 <details> 
 <summary>Desktop lightouse test results PNG</summary>

![mobile](./src/assets/images/google-lighthouse-test-desktop.png)

 </details>

 <details> 
 <summary>Mobile lightouse test results test PNG</summary>

![Desktop](./src/assets/images/google-lighthouse-test-mobile.png)

 </details>

---

## Deployment

I deployed this application was deployed using Github pages through VSocde.

### How To Run The Project Locally

1. Download the zip folder from under the code menu.
2. From your folder in the terminal git clone https://github.com/Ciaran-io/explore-ireland.git.

### How To Build Project Before Deployment

> note: Build requires Node.js 12.13.0 or higher

1. Install node modules, from the root directory run:
   ` npm install

This will download all the necessary node modules; tailwind CSS, PostCSS, autoprefixer, cssNano, imagemin & terser.

- Tailwind CSS - This allows CSS to be generated using plain HTML inside the HTML document.
- PostCSS - Preprocceor to compile CSS in javascript to CSS
- autoprefixer - Added vendor prefixes to support CSS in older browsers
- imagemin - Converts jpeg files to webp (smaller image files)
- cssNano - PostCSS plugin used to minify CSS files
- terser - Used to minify javascript files.

2. Final Build involves running 3 separate commands in the terminal to minify CSS & js files, remove unused CSS & covert jpeg images to smaller webp files.

- Minfy ccs and removes unused CSS
- To minify and remove the unused CSS that tailwind CSS provides, first go to the postcss.config file and uncomment line 5-7 that will allow CSS nano to run in the build step. Next, go to the tailwind config file and set the purge object boolean from false to true, this will purge all the unused CSS in the final build process.
  Next From the root directory run ` npm run buildcss`

<br>

- Minify javascript files

> note: The terser build script in the package.json file will need to be changed for each js file. The src input and output directory will need to be changed for each javascript file. This is inefficient, however, I have not found a way to minify all the javascript files and output multiple js files.

From the root directory run ` npm run buildjs`
<br>

- Convert jpeg files into webP files using terser. This will take all jpeg images from the source directory, change the files to webP files and output them to the dist directory

From the root directory run ` node imagein.js`

---

## Credits

### content

- The cycle location & walking trails used in google maps & the card content that displays the trail locations [sportsireland.ie](https://www.sportireland.ie/outdoors/cycling-off-road/trails)

- The top tourist locations are sourced from [Plantware.com](https://www.planetware.com/tourist-attractions/ireland-irl.htm)

Places of interest card content are based on google search results for popular tourist destinations in the selected areas

### Media

- All images are obtained from [unsplash.com](https://unsplash.com/)
  <br>

- Image: hero-image-mountain
  credit: [David Marcu](https://unsplash.com/photos/VfUN94cUy4o?utm_source=unsplash&utm_medium=referral&utm_content=creditShareLink)

- Image: cycle-route-card-image
  credit: [Gemma Evans](https://unsplash.com/photos/LTEo69JUv7o?utm_source=unsplash&utm_medium=referral&utm_content=creditShareLink)

- Image: trail-route-card-image
  credit: [Jake Melara](https://unsplash.com/photos/Yh6K2eTr_FY)

- Image: tour-route-card-image
  credit: [Luke Tanis](https://unsplash.com/photos/Vc1JoFCbym4)

- Image: galaway-city
  credit: [Kelan Chad](https://unsplash.com/photos/p7Ylyskm5Qc?utm_source=unsplash&utm_medium=referral&utm_content=creditShareLink)

- Image dublin-temple-bar
  credit: [Diogo Palhais](https://unsplash.com/photos/tnzzr8HpLhs)

- Image: dublin-temple-bar
  credit: [Diogo Palhais](https://unsplash.com/@diogopalhais)

- Image: county-calre
  credit: [Mick Haupt](https://unsplash.com/photos/P39rmORGBFw)

- All icons are sourced from [iconmoon](https://icomoon.io/)

### Code contribution

- Google maps styles
- Credit: [Mattew Pill](https://snazzymaps.com/style/287720/modest 'link to snazzymaps.com')

- Contact form, function to send an email or return a message error, or a sent message to the user after a message submission.
  credit:[EmailJs](https://www.emailjs.com)

### Acknowledgments

- Inspiration for the project [discoverireland.ie](https://www.discoverireland.ie/things-to-do/off-the-beaten-track)
