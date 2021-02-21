# Hello Chef - Frontend Assignment

## Brief

Your assignment is to create a flight search web app using Skyscanner Flight Search API.
Link: https://rapidapi.com/skyscanner/api/skyscanner-flight-search

Your app should consist of two screens and it should be powered by Vue.js.

Feel free to use any CSS framework of your choice and create the UI as per your liking. (Bonus points for making it mobile first & responsive.)

Feel free to add tests how you see fit.

## Features

1. The **index page** offers these inputs:
    - **From:** Name of the city the passenger is traveling from. It should offer an auto-suggest drop-down once two or more characters are input.
    - **To:** Name of the city the passenger is traveling to. It should offer an auto-suggest drop-down once two or more characters are input.
    - **Departure on or after:** This is a mandatory field. (Bonus: clicking on it should open a date picker.)
    - **Return date:** This is an optional field. (Bonus: clicking on it should open a date picker.)
2. Once the passenger chooses all mandatory fields and hits the **Search** button, she is taken to the listing page.
3. The **listing page** shows the list of all the flights available for the chosen cities between today and the departure date.
4. If a return date is specified, display both the departure and arrival flight lists together.
5. List filters:
    - The list can be filtered using a custom **cost filter**. You may calculate the highest and lowest cost from the data you receive at runtime.
    - The list can be filtered by **the “Direct” boolean flag** which indicates if the flight has any stops.
6. List sorters:
    - Both the list(s) can be independently **sorted** in ascending and descending order by these values:
        - Date
        - Cost
7. Make the cheapest flight(s) a bit visually prominent in the UI.
8. The listing page should allow you to choose flight(s) and **display the cost of travel**, including the selected return flight, if applicable.

## API

1. From the documentation, you may find that the **List Places API** endpoint is appropriate for populating cities in the auto-suggest drop-down on the first page.
2. To find the list of flights, use the **Browse Routes API** endpoint.
3. The **Browse Routes API** endpoint does not return the list of inbound (return) flights even if the return date is supplied. It’s up to you to figure out how to achieve this.
4. In order to use these APIs, you need to sign up on the Rapid API platform to acquire your “X-RapidAPI-Key”.
5. Generally, on a flight listing page, you would find flights for a specific day. In this assignment, we chose to display all the available flights between today and the given date.

## Submission & Presentation

1. Please create a public GitHub / BitBucket repository for your project.
2. Your repository must have a detailed README.md with instructions on how to set up & run your code locally.
3. It must not contain the words “hellochef” or “challenge”.
4. We would like you to present your work no later than 7 days from the day you receive your assignment.
5. Accordingly, please send us the link to your repository at least 1 day prior to the presentation meeting for a review.
6. The presentation would be done in these steps:
    - Run your code locally
    - Give us a UI and features walkthrough
    - Explain your code
    - Run tests, if any
