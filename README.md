# Happy Cups
## About
The Happy Cups website is a page for casual tea drinkers to learn more about tea to better understand what they are buying and encourage exploration of new teas based beverages.
This Happy cups page offers recipes, information and external links to helpful resources to achieve this.

Users of the website will find all they need to know ion the website to provide a solid elementary understanding of the tea landscape to encourage exploration including but not limited to: History, Information on tea blends and recipes.

I decided to bing this idea to life in the form of a static website when I realised I didn't understadn much about tea and what I did seem to know, seemed contrdictory.

The website encourages users to sign up to the mail list to keep up to date with new recipes and facts. 

![](assets/images/screenshot-website-preview.png)
---
## Technologies
- HTML Formatter
- Figama
- CSS
- HTML
- VS Code
- Git
- GitHub
- GitHub Pages
- convertio
- MS Word
- Material Theme Builder
- Monokai++
- Live Server 
---
## Design

### Wireframes
- The wireframe for the full website was used to develop the method to plan how to structure site content.
In completing the wireframe for the site I was able to begin development in code more effectively as I has an inital target to work towards.

- The design of the site evolved as the prodect went on. this was due to increased understanding of technical capablity with CSS, and HTML as the primary tools for this website and experimenting with layouts with Dev Tools while keeping UX in mind.

- In future projects I will use more advance functionality of design tools, to devleop a more polished design. This will minimise the amount of changes as I did find that my design evolved signifantly. In doing this I will be able to complete project more efficnetly.

- Below are the wire frames for the site:
  ![](assets/images/screenshot-website-wireframe.png)
  ![](assets/images/screenshot-website-desktop-only-wireframe.png)
  ![](assets/images/screenshot-hm-pg-wireframe.png)


### Themes
- The focus of this project being tea the selected pallet was chosen to emote calm, zen and nature.
with these aims in mind the colour pallet was chosen.
- The colour scheme of the website was created with this in mind using the the material theme builed tool as a basline and modifying the pallet to better capture the essence of the theme.
  ![](assets/images/screenshot-website-theme.png)
- The font was also selected to stay uniform with the theme as such only "Roboto" a sans-serif based font was used in the project.

### Images
- Images used in the site are royalty free or have been shared under the open source licence full refrences and credits below.

### Layout
- The layout of the website uses card components to assist with creating a streamline UX  
- The theme of the website componants was created with refrence to the  [Material Design 3](https://m3.material.io) guidelines.
- layout can be seen to persist across the entire site as shown in the pages section below
- In-additon to cards a combination of flex-box and grids were used to maintain the structure of the site
---
## Features

### Navigation  
- Navbar 

  ![](assets/images/screenshot-header.png)
  
  - Header introduces the theme of the website 
  - The navbar is fixed to allow for navigation to any page regardless of current location. 
  - The navbar is multi layer that enables users to navigate to different pages fo the same topic
  - The navbar has  active effects to help the user understand where they are in the site via persistant higlighting
  - The navbar has hover effects to hel the user navigate to the desired page via highlighting the selection 



### Pages
All pages are fully responsive on all devices down to a minimum screend width of 320px
- Home page: is a hub that directs users to other pages with enguaging layout and images.

  ![](assets/images/screenshot-home-pg.png)

- History page: introduces users to key events in the western history of tea. This page presents historical periods and events in liner order levragign a timeline.
  - Stylalised list with hover effects and psudo classes.
  - more content section to guide uses to other related pages and/or sources 

  ![](assets/images/screenshot-history-tea.png)


- Varients &amp; Blends page: provides users with information to understad about tea blends adn the factors that go into making a blend, in addttion to recommendations of brands to try.
  - flex grid and card layout 
  - more content section to guide uses to other related pages and/or sources 

  ![](assets/images/screenshot-blends.png)

- Recipes page: provides users with different recipes to try at home to broaden tea experiences
  - flex grid and card layout 
  - more content section to guide uses to other related pages and/or sources 

  ![](assets/images/screenshot-recipe.png)

- Culture: informs users about popular teas and tea cultrue in countries around the globe
  - Modified list for card contanerised style
  - Extra content delivered via iframe
  - more content section to guide uses to other related pages and/or sources 

  ![](assets/images/screenshot-culture.png)

- Sign-up page: hosts the sign up form that the user is encouraged to fill out to join the mailing list
  - Contact form with required input


![](assets/images/screenshot-signup.png)
---
## Testing &amp; Validation

- The website was tested in Chrome, Mozilla and Opera browers. All features are supported and page maintained functionallity.
- The website was tested on both desktop and mobile devices. The page is responsive to a screen width of 320px 
- Dev tools used to emulate all devices from desktop to small mobile range to secure responsiveness.
- Changes can be seen in the evolution of commits. Commits show refining of scope of project to current version.
- Accessablithy of the page was assessed using the in browser Lighthouse report. all values were in good range for accessiblity and performance. Where performance was lower it was due to the use of iframes and other content. In order to minimise file sizes webp file formats were used for most images.

  ![](assets/images/screenshot-lighthouse-index.png)
  ![](assets/images/screenshot-lighthouse-history.png)
  ![](assets/images/screenshot-lighthouse-blends.png)
  ![](assets/images/screenshot-lighthouse-recipe.png)
  ![](assets/images/screenshot-lighthouse-culture.png)
  ![](assets/images/screenshot-lighthouse-signup.png)

- [HTML Validator from w3 schools](https://validator.w3.org) was used to validate formating of HTML pages. SUCCESS on all pages
- [Jigsaw CSS validatior](https://jigsaw.w3.org/css-validator/) was used to validate CSS stylesheet. SUCCESS no errors found in file

---
## Bugs

- To enable easy user navigation the header is fixed to the screen. The navbar is made of a flex box to enable responsiveness. However, when centerd the navbar seemed to shrink at a different rate from the rest of the page resulting in a gap and inablity to use website on smaller devices.
This issue was that the nav bar was a greater sive than the viewport and when fixed the navbar was removed form the context of the page as such did not grow and shrink at the same rate acusing a gap. This was resolved by uses of overflow-x property on the html and body.

- When scrolling some elements would go over the header insead of underneath. To resolve this the z-index of the header was set very high as it should always be the top most element.
- When scrolling or loading a page lage would be significant. This was due to the abundance adn file size of the image resources used. This was resolved by removing non essential sections and changing file format to WEBP 
- Uncentered section children componants on smaller screens despite flex colunm with justified and center aligned properties. This was resolved by creating a new flex column class without the flex propertiy meaning the content would no loger arrange itself as it does in a responsive manner.

- During validation of HTML card componat with rotate on click effect produced an error. For the conlick to work the div making up the card was placed insde a label for a checkbox input so a checked psudo class could be used to transform the card - no alternative to do this effect withouth using js so on click swapped to hover which may impeed user experience but resolved validation error.
 ![](assets/images/screenshot-no-on-click.png)

- When initally deployed to github pages the file structe was different with the html pages bar index in a html folder under assets. Despite correct refrenceing and a working site when spun up on the VS Code private live server. This was fixed by placing the other html documnet in the same level as the index.html file and assets folder.
---
## Deployment
- The project was developed in VSCode to gain experence developing code in a commonly found IDE.
- I created all the basic folders adn files I needed fot the webpage including html files for all web pages, and css stylesheet.
- In VS Code after creating a new terminal the repository was inialised withthe git init command
- using git add . followed by git commit -m "inital commit" the files were staged and commited to the local repo
- In github I created a new repo for the project and linked the remote repo the the local VS code environment which enabled a CI/CD workflow for the project.

- In the project specifict github repo navigated to the 'Settings -> Pages' section 
- Selected the source to be the main branch of the project.
- Project deployed on github pages to [here](https://sabgibson.github.io/hot-cups/)
---
## Credits

### Media
- Home page:
 - 
Touareg:https://unsplash.com/photos/Bmek6EYG9Uk; https://unsplash.com/photos/Lj6OgKfNkdI
karkade: https://unsplash.com/photos/DyndLuY1rII
redespresso:https://unsplash.com/photos/K0jaKN1M1Ck
yerba mate: Photo by Los Muertos Crew: https://www.pexels.com/photo/stainless-steel-pitcher-on-table-8279918/
arnold palmer: Photo by Laurens van Riel: https://www.pexels.com/photo/mason-jar-with-beverage-1141626/
afternoon-t:Photo by Suzy Hazelwood: https://www.pexels.com/photo/tea-beside-cupcakes-1796450/
masalaa chai:https://unsplash.com/photos/zI27XpN1GdA
wh:https://cdn.shopify.com/s/files/1/0086/3449/9129/products/IMG_0898.jpg?v=1637938640
whittards: https://eu-assets.simpleview-europe.com/portsmouth2020/imageresizer/?image=%2Fdmsimgs%2FWhittard_1213980555.jpg&amp;action=ProductDetailImage
obubu logo:https://www.obubutea.com/wp-content/themes/vantage/images/logo/1920.jpg
EIC:https://www.theeastindiacompany.com/wp-content/uploads/2013/06/Logo.png
MF logo: https://commons.wikimedia.org/wiki/File:Logo_seul.jpg
Photo by Tang Don on Unsplash: https://unsplash.com/photos/OHYSVSId8mA;https://unsplash.com/photos/Jierz6cDEEs;https://unsplash.com/photos/wcGb8Y3kaSE

oolong : https://unsplash.com/photos/gT_rAfFvCyw
black tea:https://unsplash.com/photos/yQ0F0hYEApI ; https://unsplash.com/photos/yQ0F0hYEApI; https://unsplash.com/photos/osaXWN-62Os

oolong:https://unsplash.com/photos/yTEFwcLlHrU
Photo by Jose Esquivel: https://www.pexels.com/photo/food-wood-cup-dry-6351882/

Photo by Eva Elijas: https://www.pexels.com/photo/green-dried-leaves-on-ground-6087394/

Photo by Pixabay: https://www.pexels.com/photo/person-holding-sliced-vegetables-on-basket-39347/

Photo by Eva Elijas: https://www.pexels.com/photo/a-pile-of-loose-jasmine-tea-leaves-5988043/

[china brew PNG in assets/image project location - personal use licence](https://www.cleanpng.com/png-green-tea-longjing-tea-white-tea-assam-tea-tea-tea-547531/)

[green-tea-leaf](https://www.cleanpng.com/png-vine-tiger-green-climbing-tiger-wall-plant-89624/)

[green-tea-cup ](https://www.cleanpng.com/png-green-tea-coffee-herbal-tea-drink-cup-of-green-tea-90507/)
[fruit-tea-cup](https://www.cleanpng.com/png-green-tea-coffee-iced-tea-lemon-tea-png-transparen-117956/)
[cloves-spice](https://www.cleanpng.com/png-clove-indian-cuisine-spice-herb-condiment-3873986/)
[ice-tea](https://www.cleanpng.com/png-iced-tea-soft-drink-sweet-tea-lemonade-iced-tea-tr-104296/preview.html)
[tea-farm-png](https://www.cleanpng.com/png-green-tea-leaf-tea-culture-green-tea-127037/)
[china-teacup](https://www.cleanpng.com/png-teacup-teaware-tea-cup-435557/)
[china-teaset](https://www.cleanpng.com/png-teapot-matcha-tea-set-twinings-chinese-tea-751118/)
[china-teacup-w tea](https://www.cleanpng.com/png-green-tea-tieguanyin-tea-culture-u9752u8336-bowl-o-539369/)
[japan-matcha-set](https://www.cleanpng.com/png-japanese-tea-ceremony-matcha-milkshake-japanese-cu-439696/)
[japan-matcha-mixer](https://www.cleanpng.com/png-matcha-green-tea-ice-cream-japanese-cuisine-2188801/)
[tea-filter](https://www.cleanpng.com/png-tea-strainers-porcelain-mug-2738556/)
[tea-pot-kettle-fp](https://www.cleanpng.com/png-tea-egg-coffee-teapot-menu-kettle-268936/)
[spoons](https://www.cleanpng.com/png-korean-tea-tea-set-japanese-tea-ceremony-teapot-ba-353214/)
[earl-grey-filter](https://www.cleanpng.com/png-green-tea-white-tea-earl-grey-tea-tea-strainers-2378326/)
Photo by <a href="https://unsplash.com/@m_malkovich?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">petr sidorov</a> on <a href="https://unsplash.com/s/photos/incense-burner?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText">Unsplash</a>
  

[BBQ photo by Min An](https://www.pexels.com/photo/close-up-photo-of-man-cooking-meat-1482803/)

https://unsplash.com/s/photos/loose-tea

Photo by Mareefe: https://www.pexels.com/photo/peppermint-tea-on-teacup-1417945/
Photo by Eva Elijas: https://www.pexels.com/photo/a-pile-of-loose-mallow-flowers-5988312/

Photo by Quang Nguyen Vinh: https://www.pexels.com/photo/woman-picking-fruits-under-gray-sky-2153824/

Photo by Min An: https://www.pexels.com/photo/green-leafed-plant-1240961/

Photo by Pixabay: https://www.pexels.com/photo/scenic-view-of-rice-paddy-247599/

Photo by Quang Nguyen Vinh: https://www.pexels.com/photo/verdant-green-fields-in-hilly-landscape-6711568/

Photo by Quang Nguyen Vinh: https://www.pexels.com/photo/anonymous-farmers-collecting-tea-leaves-into-straw-baskets-during-work-on-plantation-4544201/

Photo by Yosi Azwan: https://www.pexels.com/photo/beautiful-scenery-of-tea-plantation-3752402/

https://convertio.co/webp-converter/

Photo by Kim Cruz: https://www.pexels.com/photo/clear-plastic-cup-with-brown-liquid-and-ice-4071422/

Photo by Dmitry Alexandrovich: https://www.pexels.com/photo/fresh-green-tea-463445/

Photo by Charlotte May: https://www.pexels.com/photo/green-tea-in-oriental-cup-on-table-5946715/

Photo by Vicky Tran: https://www.pexels.com/photo/photo-of-jar-near-cinnamon-sticks-3273989/

Photo by Charlotte May Chai: https://www.pexels.com/photo/cup-of-masala-chai-on-table-5946623/

Photo by Lisa Fotios: https://www.pexels.com/photo/photography-of-blue-ceramic-coffee-cup-734983/

Photo by Erik Mclean: https://www.pexels.com/photo/cup-of-coffee-with-milk-on-white-table-4061673/

Photo by Natalia Kretinina: https://www.pexels.com/photo/orange-ceramic-mug-with-coffee-5596479/

Photo by Jason Leung on Unsplash https://unsplash.com/@ninjason
Photo by Anastasiya Vragova: https://www.pexels.com/photo/a-person-holding-clear-glass-cup-of-coffee-7038283/
Photo by Melike  Benli: https://www.pexels.com/photo/cup-of-aromatic-camomile-tea-on-ornamental-tablecloth-10213086/

https://unsplash.com/photos/mhJODzwzCtg

https://unsplash.com/@gabimirandan

https://unsplash.com/@mmpixz

Photo by Anna Pou from Pexels https://www.pexels.com/photo/a-person-making-tea-8329270/

Photo by Ehioma  Osih: https://www.pexels.com/photo/close-up-view-of-pouring-tea-9880632/ ataya 

Photo by Charlotte May: https://www.pexels.com/photo/herbal-black-tea-pouring-into-glass-5946807/

Photo by Charlotte May: https://www.pexels.com/photo/ceramic-cup-of-tea-with-fresh-lemon-5946718/

Photo by Charlotte May: https://www.pexels.com/photo/green-tea-in-oriental-cup-on-table-5946715/

https://unsplash.com/@teacora

https://unsplash.com/photos/1S4JCCWq2mg

Photo by Ngô Trọng An: https://www.pexels.com/photo/lemon-tea-served-on-teacup-1717767/

Photo by Tima Miroshnichenko: https://www.pexels.com/photo/hand-holding-ceramic-gaiwan-and-pouring-tea-in-glass-teapot-6545346/

Photo by Tijana Drndarski: https://www.pexels.com/photo/photo-of-slice-green-apple-and-cinnamon-stick-3338676/
Photo by RODNAE Productions: https://www.pexels.com/photo/a-person-holding-a-milk-tea-6412828/
Photo by RODNAE Productions: https://www.pexels.com/photo/a-person-holding-a-milk-tea-6412830/#
Photo by Ivan Samkov: https://www.pexels.com/photo/a-woman-in-robe-sitting-at-a-table-with-tea-pots-and-tea-cups-8952605/
Photo by Oleg Magni: https://www.pexels.com/photo/cherry-blossoms-4059199/
Photo by cottonbro: https://www.pexels.com/photo/person-in-red-and-white-floral-long-sleeve-shirt-holding-white-ceramic-mug-8748542/
Photo by cottonbro: https://www.pexels.com/photo/a-performer-drinking-from-a-tea-cup-6842334/
Photo by cottonbro: https://www.pexels.com/photo/a-performer-drinking-from-a-tea-cup-6842334/

Photo by cottonbro: https://www.pexels.com/photo/man-in-red-robe-standing-near-green-trees-5385901/

Photo by Charlotte May: https://www.pexels.com/photo/
https://www.pexels.com/photo/aerial-view-of-farmland-2067255/photo-of-person-using-bamboo-whisk-on-making-matcha-drink-5946632/
Photo by Pixabay: https://www.pexels.com/photo/girl-standing-near-green-leaves-511407/

Photo by Kim Cruz: https://www.pexels.com/photo/clear-plastic-cup-with-brown-liquid-and-ice-4071422/

---
Licences &amp; Copyright
