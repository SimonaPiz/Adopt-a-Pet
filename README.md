# Adopt a Pet - Web App
> A React app to practice React Router v6

Preview at [this link](https://adopt-a-pet_simonapiz.surge.sh/)

![anteprima](https://user-images.githubusercontent.com/91121660/235917882-0f645705-805f-4dcb-a405-490e2e9e5c0e.png)

## Table of contents
* [About this project](#about-this-project)
* [Objective](#objective)
* [Technologies](#technologies)
* [Setup](#setup)

## About this project

In this project, I practice using React Router to add client-side routing to a React Application. 
I building a pet adoption website that allows users to view all the animals of a particular species and view the profiles of specific animals.

- Currently, the app renders a `HomePage`component that fetches and displays all adoptable pets.
    - **src/pages/home/index.js**
- We have also built a `PetDetailsPage` to display the details for a particular pet, but this component will not render until you create a route to display it.
    - **src/pages/detail/index.js**

> Use this database for mock data [Urgent Need for Pet Adoption - Find Dogs & Cats & More | Petfinder](https://www.petfinder.com/)

## Objective

The objective is to **add client-side routing to the application** using React Router so that:

- The `HomePage`component responds to the browser’s current URL by displaying only pets of the species the user wishes to view.
- The `PetDetailsPage`page displays when the browser’s current URL includes a specific pet’s `id`
    - It displays data for the correct pet based on the `id`in the URL parameters’ values.
- When the user searches for a pet in the search bar, they are redirected to the `SearchPage`, which uses the query parameter called `name`to filter pets by name.
- When a user clicks a pet whose details are not available, they are redirected to a `PetNotFoundPage`
- From the `PetNotFound`page, users can click “**Go Home**” button that will take them to the root path page.


## Technologies
- React 18
- React Router 6
- uses Mock Service Worker (MSW) to replicate the functionality of an external API.

## Setup
To run this project, install it locally using npm:

```
$ cd ../[directory]
$ npm install
$ npm start
```
