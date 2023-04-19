[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=10900607&assignment_repo_type=AssignmentRepo)
# Assignment Five

## REACT Website Link
https://csc3916-react-9zpc.onrender.com

## Postman Button (Assignment 4)
[![Run in Postman](https://run.pstmn.io/button.svg)](https://app.getpostman.com/run-collection/25556302-fa3940ee-4ee0-442c-b580-e2659c27a363?action=collection%2Ffork&collection-url=entityId%3D25556302-fa3940ee-4ee0-442c-b580-e2659c27a363%26entityType%3Dcollection%26workspaceId%3D40489577-8045-4fcb-a05a-12cee9fdbd45#?env%5BAbdurKhanAssignment4%5D=W3sia2V5IjoiSldUIiwidmFsdWUiOiIiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IkpXVC4uLiIsInNlc3Npb25JbmRleCI6MH0seyJrZXkiOiJVc2VybmFtZSIsInZhbHVlIjoiIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImRlZmF1bHQiLCJzZXNzaW9uVmFsdWUiOiJ1c2VyXzUwOSIsInNlc3Npb25JbmRleCI6MX0seyJrZXkiOiJyYW5kb21TdHJpbmciLCJ2YWx1ZSI6IiIsImVuYWJsZWQiOnRydWUsInR5cGUiOiJkZWZhdWx0Iiwic2Vzc2lvblZhbHVlIjoiNnhwaXZjbTBhYzYiLCJzZXNzaW9uSW5kZXgiOjJ9LHsia2V5IjoibW92aWVJRCIsInZhbHVlIjoiIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImRlZmF1bHQiLCJzZXNzaW9uVmFsdWUiOiIiLCJzZXNzaW9uSW5kZXgiOjN9XQ==)

## Purpose

The purpose of this assignment is to create a React Single Page App over your developed API.  The interface will allow the users to search for movies, display information about the movie, see stored ratings, and allow the user to enter a rating.

## Pre-Requirements
- Assignment 3 deployed REACT app that supports SignUp and Logon
- Assignment 4 that supports reviews

## Requirements
- Update your API to support storing an image (or image URL) for the movies you have stored.  You will use the image URL in your React application to show the image of movies
    - New Attribute on the movie collection
- For this assignment all your endpoints should be protected by JWT authentication
- Implement the following interfaces
    - User SignUp and User Logon
        - Leverage your User mongoDB collection to store new users of the application
    - Main screen should show the top rated movies (show at least 5)
        - Your GET /movies endpoint should sort by rating (server side)
            - Update your /movies (with reviews=true) endpoint to sort by average rating descending
    - Movie Detail screen, shows the Movie, Image, Actors that were in the movie, aggregated rating for the movie and grid that shows the reviews (username, rating, review)
    - Extra Credit: (7 points) - chapter 25 of (https://www.amazon.com/dp/B0979MGJ5J?_encoding=UTF8&psc=1&ref_=cm_sw_r_cp_ud_dp_M9YGPJNZWB3BK0P59QX3) Movie Search – show results in a grid, accordion or other list control
        - Add Search API (HTTP POST) to the API that can take partial movie names or partial actor names

## Submissions
- User is able to Sign-up (name, username, password)
- User is able to Logon to the application (username, password)
- User is able to see list of movies and select a movie to see the detail screen (top rated movies displayed)
- User is able to enter a review on the detail page (enter a rating and comment) – the logged in user’s username will be associated with the review (as captured from the JSON Web Token)

## Rubic
- -3 Not able to add comments
- -2 Not aggregating rating (average rating)
- -3 if not pointed to correct end point (e.g Hw4 endpoint)
- -5 if you don’t have a react web site deployed 

## Resources
- https://github.com/facebook/create-react-app
- https://github.com/mars/create-react-app-buildpack#user-content-requires
