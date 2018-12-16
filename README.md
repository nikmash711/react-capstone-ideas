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
Wouldn't it be nice to keep a timeline of your pet's life? From keeping track of their medical appointments to remembering something hilarious they did the other day, it can be easy to forget important things about your furry best friend.
Well now you can keep track of it all with Pawfiles! Pawfiles helps you keep a simple timeline on your pet: whether it's what the vet said at their last appointment, a record of their vaccination schedule, or a cute memory you just don't want to forget :) 

## User Stories/MVP: 
1. User can create an account for themselves with a first name, last name, username, and password
2. User will be directed to a profile page where they can add a pet and fill out basic information about their pet - breed, gender, type of animal, profile photo, brief bio, etc. (user can edit this later) 
3. Single user can have as many "pawfiles" as they wish if they own more than one pet
4. User can add a posts for each pet - if it's a memory or achievement, they can write a description and upload a photo corresponding to the memory, if it's medical/health related they can include a description of what the vet said, symptoms, labs, which vet, location (map api?) etc. User can choose a date for the post
5. Posts will be organized on the Pawfile chronologically (not according to when the user created the post but rather when the user specified the event took place)
6. User can search for posts on their Pawfile, or filter it by category 
7. There will be a sidebar on the Pawfile where the user can add a list of reminders for that pet: for example, need to buy more litter, or go get groomed next week, etc. 
8. There will be another sidebar where the user can click which pet's Pawfile they want to edit (only there if they have more than one Pawfile) 

## Extension Features: 
1. User can change their password
2. Users can see other user's Pawfiles (read-only) via a link
3. Users can edit their posts, delete their posts, update their pet's profile photo, etc.
4. Users will only be logged out after a certain amount of time, not every time they refresh
5. When requests are sent via a GET method, they will be queried to the end of the url so the user can click back or search their history 
6. Users can search for vets in their area (Yelp api?) 
7. User can directly upload a photo or file from their computer and not via an external link (that way they can upload files/records etc.) 
8. Reminders can include a time, and can even push notifications to the user (to their notification center or via text/email) - like for daily pills 
9. Use some of these pet puns throughout the app: https://www.lifelearn.com/2016/02/24/the-jumbo-reference-list-of-pet-puns/
10. Page puns/design will depend on whether it's a cat, dog, or other. and if it's male/female

## Foreseeable Issues: 
1. Storing images/files in MongoDB (I think I'd have to use something called GridFS) 
