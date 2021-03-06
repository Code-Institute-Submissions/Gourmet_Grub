## GourmetGrub Testing

### Manual Testing

### **Planning**

------

The main goal of this website is to offer users a quick and simple way to easily access, add, share or update cooking recipes in an interactive manner. This testing will be carried out using developer tools audit tests, different browsers and also different screen sizes to check responsiveness. Validation tools and automated tests will also be carried out to check the code's validity, as outlined in the "Automated testing" section below. The main means of testing the intended purpose of this website will also be to go through each client story and check if their outcome was achieved.

### **Implementation**

------

#### Manual Tests

##### *Methodology used*

*This site was tested across the below browsers:*

- Chrome
- Safari
- IE
- Firefox

*And devices:*

- Laptops (windows & mac)
- Desktop (windows & mac)
- iPhones 5 & 7,
- iPad & iPad mini
- Samsung's 6, 8, 10 & A7

The audit tool from google inspect was also used in order to improve on three aspects:

- Performance
- Best Practices
- Accessibility

###### *Manual tests carried out*

**Common elements:**

<u>Navbar</u>:

1. Confirm nav is a list of the different pages on md-xl screens
2. Confirm nav is a burger icon with collapsible menu on xs-sm screens
3. Confirm current page is highlighted in the nav menu
4. Confirm nav items and nav search icon changes colour when hovered over
5. Confirm user is brought to correct page for each nav item
6. Confirm that when clicked the nav search icon calls an overlay covering the screen
7. Confirm that the form searches for the entered string when button is clicked or 'entered' typed
8. Confirm that incorrect spelling is highlighted 
9. Confirm user is redirected to page of the results with the matching recipes
10. Confirm user is redirected to null results page if no matches

<u>Float Top Button:</u>

1. Confirm button only appears on bottom right of screen when user has scrolled down the page
2. Confirm that the icon changes colour when hovered over
3. Confirm that the user is brought to the top of the page when button is clicked
4. Confirm that the action of scrolling to the top is  slowed down and not a sudden jolt
5. Confirm icon is above any content that is on the page and doesn't have a lower z-index

<u>Error 404:</u>

1. Confirm if an error occurs that the use is returned correctly to the error page, from all pages

**Index/Home Page:**

1. Confirm that the page content is centered on all screen sizes
2. Confirm that the opacity of the form changes when the user clicks on the form area
3. Confirm the placeholder text is replaced by user's input when types
4. Confirm incorrect spelling is highlighted on the form if input is left as is
5. Confirm user is redirected to matching results page for inputted string
6. Confirm user is redirected to null results page if no recipes match search
7. Confirm background picture is clear, sharp and loads well
8. Confirm placeholder content is fully visible on small phone screens

**Cuisine Page**

1. Confirm user is shown all results from the DB of cuisines in it
2. Confirm there are no duplicate results on the page
3. Confirm that on smaller screens the text font size isn't too big and out of place
4. Confirm that each row containing the cuisine obtains a gradual box shadow on hover
5. Confirm if there are no cuisines the user is redirected to null results page
6. Confirm 'view all' button highlights gradually on hover
7. Confirm the 'view all' button redirects the user to another page with recipes with the same cuisine

**Meals Page**

1. Confirm that content is centered on all screen sizes
2. Confirm that the title and form content doesn't skew on smaller screens
3. Confirm that the user is presented with the 3 options when they click the dropdown
4. Confirm that the option the user just chose is now the selected option
5. Confirm that when the 'fine meals' button is clicked  the user is redirected to a page which contains the recipes with the matching meal type searched
6. Confirm the user is redirected to null results page if there are no matching recipes

**Add/Edit Recipe**

1. Confirm all forms are centered on the pages and placeholder content is visible
2. Confirm placeholder content is hidden but scrollable if it goes over the form input's length
3. Confirm that when an input is clicked the form bottom border highlights
4. Confirm placeholder content is positioned to the left of the form input field
5. Confirm that the icons place correctly and proportionally to the left on all screen sizes
6. Confirm that the meal type dropdown highlights on hover
7. Confirm all form min and max fields are working correctly
8. Confirm user can't input characters into calories and duration form fields
9. Confirm user can't input incorrect non url/picture file string type into image input
10. Confirm user can not add/save recipe without entering inputs into all form fields
11. Confirm modal is called when ingredients or prep steps inputs are clicked on
12. Confirm user can add extra form fields in this modal as they need them
13. Confirm user can delete the form fields in the modal but there will always at least be one
14. Confirm max number of inputs is 20 and user is alerted when this is reached
15. Confirm that when in edit page, all the existing data is displayed correctly
16. Confirm that when a recipe is added the user is redirected to a thank you page showing the recipe just added
17. Confirm 'cancel' button brings user back to the all recipes page

**All Recipes Page**

1. Confirm that results are displayed 6 at a time in a vertical card format on all screens
2. Confirm that BS4 is adhered to and 3 are displayed on each row
3. Confirm that on smaller screens the columns take the full width of the screen each
4. Confirm that the card text and button is centrally aligned on medium to smaller screen, but left aligned on bigger screens
5. Confirm the text does not overflow its div anywhere on the cards on any screen
6. Confirm cuisine type shown in bottom left of the footer is correct
7. Confirm views are floated to the right side of the footer correctly
8. Confirm that when a card is hovered over the card's background changes cover slightly and slowly
9. Confirm the button changes colour slightly and gradually when hovered over
10. Confirm that on click the 'view full recipe' button will redirect the user to the correct chosen recipe
11. Confirm that once the user goes back to all recipes the 'views' field has updated correctly on the recipe
12. Confirm pagination updates correctly if more recipes are added to the DB
13. Confirm user is brought to the correct page number they click on

**Meal/Cuisine/Search results page**

1. Check that searched term is the title of the page
2. Check that cards are displayed horizontally in rows 
3. Check that cards contain their name, description, views and cuisine fields, and its picture
4. Check that none of the text goes over their div and is hidden if they do
5. Check that the entire card is highlighted when hovered over
6. Check that picture goes on the top of the card when screen size is smaller
7. Check that results are sorted correctly by their number of views
8. Check that clicking the 'view full recipe' brings the user to the correct recipe page
9. Check that by clicking the 'back' button the user is brought to the previous page

**Single Recipe Page**

1. Confirm that on smaller screens the columns are displayed in full width, taking a row to themselves
2. Confirm that the correct recipe heading is displayed at the top of the page
3. Confirm that recipe ingredients are shown on the left hand side but the text is right aligned
4. Confirm the summary stats under the recipe picture are indeed correct
5. Confirm the steps are fully shown and displayed on all screen sizes
6. Confirm that clicking on either of the social media share buttons redirects the user to their social media page with a chance to share the recipe
7. Confirm clicking the edit button brings the user to the correct recipe's edit page
8. Confirm clicking the 'back' button returns user to the previous page.

##### *User Stories tests*

1. As a new visitor to the website, I want to be easily navigate the site to find information I was looking for in one or two clicks when searching.
   - The navbar is very simple to use and brings the user to any part of the page when clicked.
   - There are also buttons all over the page linking intuitively to different parts of it.
   - The search icon can be clicked from any page and lets the user search for any recipe in two clicks.
2. As a user, I want the different recipes to be presented to be in a tidy and easily readable manner when browsing them.
   - Recipe results from the search functions are laid out in a list form one by one as rows going down the page, the user can just scroll through the results and click on a recipe they want to see more of.
   - Recipes in the 'all recipes' page are laid out in 2 rows x 3 columns, 6 recipes per page format which doesn't take up too much screen space on either mobile or bigger screens.
   - Pagination is utilised on the 'all recipes' page to display 6 recipes at a time, making the loading process quicker and the browsing experience more pleasant. 
3. As a user, I want be able to find a particular recipe quickly by searching the word or a character string when I know what I want.
   - The index page has a search bar which will search the entire DB for any matches of the string inputted, it doesn't have to be an exact match and the results are returned on a new page.
   - The navbar also has a search icon on all screen sizes that can be accessed form any page which when clicked will call an overlay with a search bar that has the same functionality as the index search bar.
4. As a user, I want to be able to search by a food type or even meal type when I am less sure of what recipe I desire.
   - For searching for food type or 'cuisine' there is an option on the navbar which will return all the different cuisines present in the DB in a list format. If recipes have matching cuisines then the results don't repeat, instead there is an option to explore all the recipes which have this cuisine in them and that page is then returned when that button is clicked. 
   - For searching for 'Meal Type' there is another page which has a dropdown so the user can select either 'breakfast', 'lunch' or 'dinner'. Once one of these options is selected the page returns the matching recipes in a list format similar to the one seen in the cuisine results page mentioned above. 
5. As a user I want to be able to know exactly what page I am currently on when browsing the site.
   - The navbar uses jinja and pulls from the backend to know which nav-item to apply the 'active' class to, highlighting the page the user is currently on.
   - The title of the page is also added to with a '/page id' added to the head title, showing the user again which page they are on.
6. As a user, I want important pieces of info like cuisine type to be presented to me without having to click into it, when browsing through the different recipes.
   - For the search results pages jinja is used so that all the pages return the same card template for displaying important recipe info. This info consists of the title, a picture, a short description, the cuisine type and how many views it has received as outlined here.
   - For the 'all recipes' page the cards display the exact same information but in a different manner, these cards are more vertical whereas the prior mentioned cards are horizontal
7. As a user, I want the recipe I decide on to be easily readable and followable step by step when reading it.
   - The single recipe pages is very clear and concise and well laid out for a user to view/follow. It only displays the important information such as; picture, ingredient steps, preparation steps and quicks summary stats for the recipe, duration, calories and number of ingredients.
8. As a user I want to be able to share this recipe on my social media platform when I am happy with the results of cooking it.
   - There are two social media links which allow the user to 'post' this recipe to the social media site of which they desire.
9. As a user contributing to the site, I expect a certain level of feedback to confirm that my work was submitted successfully, such as a thank you page.
   - When a user submits a recipe to the page a 'thank you' page is returned showing the full page of the recipe that they have just added.
10. As a user browsing the site, if there are no recipes matching my search I want a page returned confirming this, not just an empty page.
   - When no recipes are returned either from an empty DB or from a no results search the user is redirected to a template stating this, instead of just an empty page.
11. As a user, I want this site to be mobile/tablet friendly and be just as responsive as a desktop site would be when using this site on a mobile phone, as you more that likely would in a kitchen.
   - The BS4 classes and layout were utilised in this project to have the layout responsive to different configurations etc. 
   - Media queries were used for heading font sizes on smaller screens and positions of items. CSS such as 'text-overflow' was also used to hide any text that goes over its div.

### **Results**

------

##### *Results of Google Audits*

This let me realise where aria-labels were missing and alt tags, along with labels for forms and if CDN library version was vulnerable. Where loading times can be reduced and colour's opacities needed to be changed to improve performance. The pictures were gotten from [Pexels](https://www.pexels.com/) and were already small in file size so didn't need to be condensed further.

##### *Bugs fixed*

Most of the issues that were on the page stemmed from the initial adding of the recipe to a page from the 'Add Recipe' form, these are as follows:

Recipe description, titles and cuisine over running their divs on the page. There were several cases on the page where a title may have been too long or the description text of the recipe over ran its div. These bugs were corrected with form validations on the add page. The 'pattern' and 'maxlength' attributes were utilised for this, along with 'required' (which was used on all forms) to ensure that an empty string was not entered. The divs were also given fixed heights and the text overflow in the y direction was hidden.

Errors were being thrown up across the page when searching for recipes as there were 'no results' being returned even when the string was correct. I came to realise that this was an issue with capitalization of the strings inputted. This was corrected by using 'IGNORECASE' for my regex in the backend function and also a JS function of which capitalized the first letter of the string inputted and made the rest lowercase, thus returning all matching recipes.

This function then unearthed an issue with the backend code for adding/editing recipes. The 'type=number' attribute was being used for number inputs, which threw errors in the console when the 'Caps' JS function was used on them as they were not strings. To correct this error I only used the caps function on the string form inputs, but I also realised that the form inputs were being uploaded to the DB as strings in the backend, this was corrected by wrapping the values in int() to make them an integer.

There was also an issue with the system for uploading pictures along with the recipe, as no file was being displayed sometimes. To correct this, the type was changed to 'URL' and the pattern attribute was used to ensure that he string ended in an image file type, i.e. JPG, PNG or gif.

When searching for a recipe, or indeed any recipe in the 'all recipes' page, there was no page loaded for no results or if the DB is empty. This was corrected by adding a 'Null' html page to redirect to if that is the case, encouraging the user to add a recipe. This was also a similar case for when adding a recipe, the user wasn't notified of their successful add. This was rectified in the same manner by redirecting the user to a page saying thank you and showing the recipe they have just added below.

The form for 'Meal type' threw up a few issues as the user was able to search when there was no meal selected, so recipes with no meal type would be returned. The other issue was that when a recipe was edited, the meal type would reset to none, which gave results for the incorrect 'none search'. To correct this I created a jinja if/elif/else statement in the edit page to denote the 4 different situations; breakfast, lunch, dinner, none. Gave the first empty option an empty value and attributes selected, hidden, disabled and required. This would mean the user can't select none and the form won't reset itself due to the jinja statement as it finds which type of meal it is. The attributes were also added to the 'add recipe' form and 'meal results' page form for searching meals, this eradicated the 'none' option and the meal types were correctly maintained or edited on the recipes.

An issue became apparent with the 'views' field, it was updating correctly when a recipe was viewed in its own single page, but when this recipe was edited the 'views' field reset back to 1, as it was when first added to the DB. This was corrected by using the '$set' operator to only update the fields that were outlined in it, which was every other field apart from 'views'. The recipe views now increments correctly when the recipe is viewed and doesn't change when it is edited.

The 'back' or 'return' buttons used on some pages caused issues as they were wired up to return to a certain page, however some pages have many different routes or avenues to get to them. A JS function was made to fix this where the it just brings you back a page in the browser history. This functionality was added tp the buttons needing it and when clicked they called the function.

Issues with screen sizing and layout became apparent in the testing of this page mainly with the smaller screen sizes. The BS4 col sizing was used to rectify these errors and ensure the elements are positioned correctly. For font issues on smaller screens media queries were used.

When an error occurred with the running of the page it just retuned you to an 'error 404' page for example. A function was implemented into the back end to catch and create a route for these errors and return a page to bring you back to the home page.

##### *Bugs still an issue*

There was an bug in IE where the JQuery used doesn't work, I looked up [Can i use](https://caniuse.com/#search=jquery) and unfortunately it isn't available in any forms of IE.

### Automated Testing

#### Validation

- [W3C Markup Validation](https://validator.w3.org/) was used to validate HTML.
- [W3C CSS validation](https://jigsaw.w3.org/css-validator/) was used to validate CSS.
- [JSHint](https://jshint.com/) was used to validate JavaScript.

#### Jasmine

The main functions were tested in this project with Jasmine as a means of ensuring they were working as planned. The way I approached the testing method was to start small and make sure it is implemented correctly in the first place and work from there. As I am new to Jasmine testing this method best suited me for this project. The files for testing are below:

- [Jasmine HTML](https://github.com/brianscan14/Gourmet_Grub/blob/master/testing/jasmine/jasmine.html)
- [Jasmine JS specs](https://github.com/brianscan14/Gourmet_Grub/blob/master/testing/jasmine/jasmine.spec.js)
- [JS](https://github.com/brianscan14/Gourmet_Grub/blob/master/static/js/script.js) 

###### Running the tests

Firstly make sure the the project is cloned from the GitHub repo and running on your own IDE as outlined in the [README.md](https://github.com/brianscan14/Gourmet_Grub/blob/master/README.md) file. Then:

1. Open the Jasmine HTML file.
2. Run it to see the results in your browser.

To create Jasmine tests of your own:

1. Open the Jasmine spec file.
2. Write the tests using Jasmine's framework.
3. Save the spec and refresh the HTML file.

#### **Python**

The file test was my [app.py](https://github.com/brianscan14/Gourmet_Grub/blob/master/app.py) file and the code was run in the [test.py](https://github.com/brianscan14/Gourmet_Grub/blob/master/test.py) file.

###### How to run Python test

Firstly make sure the the project is cloned from the GitHub repo and running on your own IDE as outlined in the [README.md](https://github.com/brianscan14/Gourmet_Grub/blob/master/README.md) file. Then:

1. Open the [test.py](https://github.com/brianscan14/Gourmet_Grub/blob/master/test.py) file.
2. `cd` to the correct directory in the terminal and then enter (your command may differ):
   - `python3 test.py`
3. The terminal will print out that all the tests passed if they are passing.