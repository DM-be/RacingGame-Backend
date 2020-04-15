# RacingGame-backend
The backend .NET core project built for the racing game project in the foundation .NET course.

## Description
A Unity racing game was made for the foundation .NET course. The game features a login system that keeps track of a user's score. These scores are kept as "highscores" in a database. These highscores can be viewed on a [frontend](https://github.com/DM-be/RacingGame-frontend) hosted website made in Angular.

## Technical

For this project I was responsible for the backend implementation of the score and login system. The login system is implemented with JWT token verification.
The Unity client registers and logs in users, receives the token, stores it client side and sends it with each request. 
The controller in this backend verifies the token before adding a score in the database. The database is integrated with Entity framework. 


SignalR is integrated within this project to provide the frontend with realtime highscores when users play the game, without the need for refreshing.
I [implemented](https://github.com/DM-be/RacingGame-frontend/commit/8c2a0d6d12699c404795524688db8768efc632b6) this feature in the frontend.


