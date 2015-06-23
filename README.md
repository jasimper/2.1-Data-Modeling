# Data Model for Picture App

Below are the neccessary Classes with attributes for the app.

### User
* username
* password
* first_name
* last_name
* picture_id [](links to instances of Pictures class)
* comment_id [](links to Comments class to show all comments made by user)
* group_id [](links to Group class to access groups you are a part of)

### Pictures

* user_id (links to instance of User class aka Image poster)
* image
* title
* location_taken
* timestamp_taken
* timestamp_posted
* additional_notes
* tag_users
* comment_id [](links to instances of Comment class)

### Comments

* picture_id (links to Pictures class)
* user_id (links commenter by their instance of User class)
* content (the actual comment)
* timestamp_posted

### Group/Family

* user_id [](links with User class to show group members
* group_name
* group_description
