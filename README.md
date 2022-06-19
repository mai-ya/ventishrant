# VENTISHRANT
## Video Demo: 
## Description: 
This is my final project to conclude CS50x. I used the python and html/css taught in later weeks and tried making the project with Flask (week 9), but decided to challenge myself by programming the final result with Django, a different web framework. 
### Why Django? 
Django has some neat built-in features like a superuser and admin page. I also wanted to challenge myself as I explored Flask a lot in the Week 9 Problem set already. Afterall, part of CS50X's goal is not only to teach you to program but also to teach you how to learn to program yourself. 
### Why "ventishrant"?
I often check online forums like "AoPS" and "StackExchange", but found that these are too educational for venting. On the contrary, "Ventishrant" is a platform for students to share stories or essentially anything making them unhappy without revealing their name or school etc. Instead of finding something to help students "brighten their day", ventishrant is simply a place where they can flush out bad emotions and hopefully guide themselves into clearing away bad memories. 
### Website Info & Description
Overall I like to keep my website simple and clean!
#### Home page
The home page displays all the rants that any user has posted. I have created a paginator which neatly displays the current page (there are five posts on each page), the 3 pages before/after it, and the first and last post. I have also truncated the characters to - 200 so that no post can clog up the page. 

### Post Detail 
If you click the heading of a post in the home page the website redirects you to a more detailed page where you can comment on a post or, if you are the post's author, edit/delete the post. If the post is longer than 200 characters the detailed post page is also where you can find the full length of the text. The path of these pages are localhost:8000/post/id where the id is the post_id stored in the local database.

### Usage
This page is quite simple and not exactly "responsive", it just tells users how the website works. Now that google doesn't have a "lower security" account option (something along those lines) I cannot have Django send emails with its default passwordresetview with my email address being the sender. Unfortunately it fails its authentication and thus the "passhint" and "passanswer" is the only way a user can reset. 

### Announcements
This page filters posts so that only ones posted by staffs are listed. If some of the posts from staffs are vents themselves, I could create a new staff account specially for posting announcements. Possible announcements include new features, site updates, and fixed errors/bugs. 

### Editing Profile
The user can edit its profile image and the default email through the userupdateform and profileupdateform. The profile image defaults to a discord cookie emoji and the ability to edit that without going to the admin dashboard page is important. The website doesn't ever ask the user for their real name and this keeps a nice degree of anonymity for a venting website. 

### Login/Logout/
The system saves a salted and hashed version of the password and users can log in or out with their password and email. 

### More Backend
I often use the python manage.py shell in my terminal to make sure everything's working well. There are added features like the profile image and passhint/passanswer which are created by making a new model - Profile with a onetoone user correspondence to the default User model. 

### Beyond CS50
Right now this is still a local project but I plan to add some more features and publish it using heroku later, perhaps after finishing CS50W. Overall, I just want to say thanks to all the CS50 staffs and discord users who have helped me along my away!
