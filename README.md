# Capstone Project - Design Desicions Report

Uluhan M. Orhan

040997625

Project: Astronomy Picture of the Day Search

**Design Desicions Report:**

 - I prefered a dark background with blurred astronomic photos to have a feeling of the space.
 - The website has three main pages. The first one is welcome page. In this page users have to pick a date to continue and see the picture.
 - The second one is the information page of the picture that is picked. There is a heart icon under the picture to add the picture to the favourites. They can also pick a new date from date picker located under the picture.
 - There are two buttons on the navigation bar; "Home" and "Favourites". The Home button redirects to the Welcome Page to let users pick a new date.
 - The "Favourites" button on the navigation bar goes to the favourites page where the users can see their favourite pictures.
 - Clicking on the heart icon on a favourited picture will remove the picture from the favorites.

**Part-3 Changes**
- I made the login page first. I most difficult part was making the background blurred. Then I gave up on this design.
- I decided to make some changes on my initial design/mockup.
- I will make the button look better and add more spice in the design.
- I forgot to switch the branch first. When I realized I worked on the wrong branch, i moved the files to part-3.

**Part-4 Changes**
- Javascript file was created and necessary HTML elements stored into the variables.
- A 'click' event listener added to the $favorites variable which holds the favorites list item with an heart icon in the index.html page. The event listener runs the showFav() function.
- Instead of having 3 different HTML pages, I just made one HTML page. The showFav() function is created to display the stored images in the page. First, the function gets the stored data from localstorage. If there is any data, and we turn them back to an array from string with the JSON.parse method. The empty HTML array is created inside the function. First I pushed the title into the array, then with iterating over the items in the favorites array the HTML structure is pushed into the HTML array. Then, all the HTML structure is stored into the $favs variable with join() method. $fav variable holds the div that displays favorite images on the HTML page. Finally, I changed the innerHTML of the $content variable with an empty string. So, only the div that holds the favorite images will be displayed on the page.

**Challenges**

- In the first design of the website, I had 3 different pages. I also had a hamburger menu on the mobile/tbalet version. I did delete them to reduce the amount of work and focus on the required things of the assignment.
- Another challange was trying to figure out how to show only favorite images when user clicked on the favorites icon on the nav. I solved it with changing the innerHTML with an empy string when user clicks.
