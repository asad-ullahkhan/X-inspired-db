# X-inspired-db
# Social Media App ERD Project

## Project Overview
This project involves designing a database for a social media application inspired by X (formerly Twitter). The goal is to model core functionalities such as user accounts, tweets, comments, likes, subscriptions, and followers using an Entity-Relationship Diagram (ERD). The ERD provides a clear structure for organizing and managing data, ensuring scalability and efficient storage of user interactions.

## ERD Breakdown & Explanations

### Users Entity
The *users* entity represents all registered members of the platform. Each user has attributes such as ID, username, and email. Users engage with the system by creating tweets, posting comments, following other users, and liking content.

### Tweets Entity
The *tweets* entity holds user-generated posts. Each tweet includes a unique ID, a user ID linking it to its creator, and its content. Tweets can receive comments, likes, and media attachments.

### Comments Entity
The *comments* entity stores reactions left by users on tweets. Each comment is associated with both a user and a tweet. Comments themselves can be liked as well.

### Likes Relationships
Likes are represented as two separate relationships:
- *Users like tweets*
- *Users like comments*

These relationships show user engagement with content across the platform.

### Media Attachments
The *media* entity stores information about files attached to tweets, such as images or videos. Each media item contains a file URL and is linked to a specific tweet.

### Subscriptions
The *subscription* entity keeps track of premium user memberships. Each subscription entry includes a start date, end date, and subscription type, and it is linked to a specific user.

### Follow System
The *follows* relationship handles user-to-user connections, allowing one user to follow another. This relationship models the social networking aspect of the platform.

## Assumptions & Constraints
- A user must exist before creating tweets or comments.
- Subscriptions are optional and only apply to users who opt in.
- Likes are only counted once per user per tweet/comment.
- Follow relationships cannot link a user to themselves.

## Group Members
| Name | GitHub Link |
|------|-------------|
| MUHAMMAD ABU BAKAR | [Profile](https://github.com/MuhammadAbuBakarQureshi) |
| ASADULLAH KHAN | [Profile](https://github.com/asad-ullahkhan) |
