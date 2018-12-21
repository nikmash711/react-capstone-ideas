# RecommendIt

## Summary of App:
Have you ever used Goodreads and thought "hey this is pretty awesome, but I wish I could recommend things other than books" :( If so, then this is for you! RecommendIt is the perfect way to not only keep track of things you've done and want to do, but to see what you're friends are recommending as well! From books, shows, movies, articles, games, places, etc. - you name it, you can RecommendIt.

## User Stories/MVP: 
1. Users can sign up with their first name, last name, username (unique), and password to join the RecommendIt social network.
2. Users can log in with their username and password. After logging in, users will be directed to their profile page.
3. Users can add a Tryit or Doneit on their profile page - DoneIts refer to things they've already done and want to rate/recommend, TryIts are things they haven't done yet but want to do. 
4. User's can report an issue from a link in the footer that will send me an email letting me know what the issue is. 
5. Users can find and click on another user's profile  to view their TryIts and DoneIts 
6. Users can delete and edit their own TryIts and DoneIts 
7. Users can pin another user's TryIt or DoneIt to add it to their own list 
8. User can filter on their profile page to only see their TryIts, DoneIts, pr a subcategory (book, show, movie, etc.). They can also search for a specific TryIt or DoneIt on their page. 
9. Users will have a navigation bar on every page after they log in with a search input, logout button, settings button, and profile page button.
10. Users can search for friends and see their recommendations via a search input on the navigation bar. On typing in the search input, other users will show up in the search results. To view more they can click "see more" and be guided to a new page with the search results matching that name. Search results will be based on whether or not search term matched first name, last name, or username of the user.


## Extension Features: 
1. Users will have an account settings page where they can add a profile picture (and be able to change it), as well as the ability to change their name or password 
2. Users can follow and unfollow each other
3. Users can comment on each other's TryIts and DoneIts
4. Users profile page will show who they follow and who follows them
5. Users will have a feed page where a list of recent recommendations from those they follow will show up, along with a "see more" on the bottom to load more.

## Foreseeable Issues: 
1. It will be challenging to structure the database since it's a social network 
2. Storing images in MongoDB (I think I'd have to use something called GridFS) 
__________________

# Pawfiles

## Summary of App:
Wouldn't it be nice to keep a timeline of your pet's life?
From their medical records to remembering something hilarious they did
the other day, it can be easy to forget important things about your
furry best friend. Well now you can keep track of it all with
Pawfiles! Pawfiles helps you keep a simple timeline on your pet:
whether it's what the vet said at their last appointment, a record of
their vaccination schedule, or a cute memory you just don't want to
forget, this is the place to document it all :) P.S. When looking at
wireframes, please look at desktop version first since I've included
descriptions of each page there.

## User Stories/MVP: 
1. User can create an account for themselves with a first name, last name, username, and password
2. User will be directed to a home page where they see all their pets (if any) and can add a new pet pawfile by filling out a form (name, species, breed, gender, profile photo, brief bio.). User can edit Pawfile’s basic info later 
3. Single user can have as many "pawfiles" as they wish if they own more than one pet
4. User can add posts for each pet - it can be a memory post with a title, description, date, and a photo URL corresponding to the memory, OR a medical related post where they can include a title, description, symptoms, labs, vet, location (maps api to make it load as they type?), date, and a link to a file. Once posted, only the info filled out will show (empty fields will not be displayed). User chooses the date.
5. Posts will be organized on the Pawfile chronologically (not according to when the user created the post but rather when the user specified the event took place)
6. User can search for specific posts on the Pawfile, and filter it by category
and/or date 
7. There will be a sidebar on the Pawfile with a brief bio about the pet as well as a list of reminders for that pet: for
example, need to buy more litter, or go get groomed next week, etc. User can add/delete reminders to this list 
8. The URL of the image the user links will show an actual image once posted, and the user can click on that image to see an enlarged version of it.
9. Navbar with Home/Py Pets - that takes you to the pet's profile, Settings, Logout 


## Extension Features: 
1. User can change their password
2. Users can see other user's Pawfiles (read-only) via a link
3. Users can edit their posts, delete their posts, update their pet's profile photo, etc.
4. Users will only be logged out after a certain amount of time, not every time they refresh or leave the browser (implement auth stuff) 
5. When requests are sent via a GET method, they will be queried to the end of the url so the user can click back or search their history (use React Routers) 
6. Users can search for vets in their area (Yelp api?) 
7. User can directly upload a photo or file from their computer (for posts or profile photo) and not via an external link (that way they can upload files/records etc.) Can do this by either using GridFs, or saving that file to another db (like AWS), and storing a ref to it in my db. 
8. Reminders can include a time, and can even push notifications to the user (to their notification center) - like for daily pills 
9. Use some of these pet puns throughout the app: https://www.lifelearn.com/2016/02/24/the-jumbo-reference-list-of-pet-puns/
10. Parts of the design (and puns) will change based on whether it's a cat vs dog, male vs female. Design will hopefully look like an actual timeline
11. "See more" at bottom of timeline to load more posts so db doesn't load all of them at once
12. Make it an app for flex week!
13. Ability to change password when logged in
14. Ability to reset password (this would involve storing user's emails, a security issue. Or they would have to report a problem, and then I'd need some way of verifying their identity). https://nodemailer.com/about/, https://www.mailgun.com/blog/how-to-send-transactional-email-in-a-nodejs-app-using-the-mailgun-api, https://www.w3schools.com/nodejs/nodejs_email.asp

## Foreseeable Issues: 
1. Storing images/files in MongoDB (I think I'd have to use something called GridFS) 

## Competitors:
1. Vitusvet (mobile app)
2. Petly (web app) 
