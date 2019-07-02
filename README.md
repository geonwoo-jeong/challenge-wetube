# challenge-wetube

## Day4

https://codesandbox.io/s/day-four-blueprint-i2mny

## Day5

https://codesandbox.io/s/express-blueprint-lo75y

Challenge goals:

아래 주어진 컨디션들을 모두 수행하여야 코딩챌린지를 통과할 수 있습니다.

Using the provided blueprint build a server that has the following routes:

```
/
/join
/login
/confirm-account
/courses,
/courses/new,
/courses/mine
/api/documentation
/api/v1/buy
/api/v1/refund
/api/v2/remove
/api/v2/edit
```

Conditions

Those URLs should be divided in 5 different routers. Each route needs to have a controller function imported from a "controllers" file.

Anonymous functions are not allowed

## Day6

https://codesandbox.io/s/express-pug-blueprint-um54k

```
Challenge goals:
아래 주어진 컨디션들을 모두 수행하여야 코딩챌린지를 통과할 수 있습니다.

Using the provided blueprint and following the MVC pattern build a server that has the following 4 routes: "/", "/login", "/photos", "/profile"
Each of these routes should render a template.
Put the templates on the 'views' folder
All templates should extend from a layout
The layout should contain the <head> portion of the page and a <footer> partial.
On the <body> each page has to have a <h1> with the title of the page.
On the <head> each page has to have a <title> with the title of the page and the title of the website
The title of the page and the website should not be written on the template.
The title of the page should come from the controller.
The title of the website should not come from the controller, it should come from the locals
There should be one router file and one controller file.
Middlewares should have their own file.
Anonymous functions are not allowed
```

## Day12

https://codesandbox.io/s/express-controller-blueprint-fo8p1

```
샌드박스 안에 db.js 라는 이름의 파일이 있습니다. 그 파일은 영화의 DB를 시뮬레이트 합니다. 아래와 같은 4개 함수를 export 합니다.
샌드박스 안에 movieController.js 그리고 movieRouter.js 가 있으며, 이는 3개의 routes 와 3개의 controllers 를 갖고있습니다.
Controllers와 Routers를 추가하거나 제거해서는 안됩니다. 단 3가지만으로 아래 챌린지를 수행할 수 있어요.
getMovies,
getMovieById,
getMovieByMinimumRating,
getMovieByMinimumYear
함수 4개에 대한 설명은 아래와 같습니다.
getMovies returns an array of movies, console.log the result to see the shape of the object.
getMovieById returns a movie object. It requires an ID as an argument and if no movie is found it returns undefined
getMovieByMinimumRating returns an array of movies, it requires a number, with this number the function will return an array of movies with a rating equal or higher than the number.
getMovieByMinimumYear returns an array of movies, it requires a number, with this number the function will return an array of movies with a release date equal or higher than the number.
코딩챌린지 수행조건
Complete all the controllers
Use pug and mixins to render pages and loop over the movies list
Use templates
You can only have 3 .pug pages. movies.pug, 404.pug, detail.pug
**Use middlewares to add locals like (siteTitle)
아래 3개의 페이지를 만드세요.
(1) Home page (/):
Render to movies.pug
The home controller has to render a page with all the movies from the db.
Use mixins to render the movies
Use the function getMovies. This is how it should look:
homeController

(2) Movie Detail (/1234):
Render detail.pug
When I click on the title of the movie I should go to /:id, for example, /1234, that page should render a detail of the movie. Use the function getMovieById. Render the title of the movie, the synopsis, and loop over the genres of the movie.
If no movie is found you need to render a 404.pug.
detail.png

(3) Movie Filtering (/filter?year=2010, /filter?rating=7.8):
Render movies.pug
Use mixins to render the list
You have to get the query from the URL and find out if the user is filtering by year or rating.
You have to use getMovieByMinimumYear and getMovieByMinimumRating
This is how it should look if I'm filtering by year:

```

## Day 16

https://codesandbox.io/s/day-eleven-blueprint-0mpl9

```
Challenges
You need to create the route, controller and .pug template for the page /add
The /add page should be a form with three inputs: title, synopsis, genres. title and genres should be inputs and synopsis should be a textarea.
This form should POST to a page with a controller that calls the addMovie function and adds the movie with the fields from the form.
The addMovie function takes one argument, that argument should be an object containing title, synopsis, genres. For example:
const movie = {
title: "Godfather", // Should be a string!
synopsis: "It's great", // Should be a string!
genres: ["Drama", "Action"] // Should be an array of strings.
}
addMovie(movie)
After the movie is created the user should be redirected back to /
Conditions
아래 주어진 컨디션들을 모두 수행하여야 코딩챌린지를 통과할 수 있습니다.

You can create a maximum of 2 controllers, bonus points if you do everything only creating 1 controller.
The form has to do a POST request.
Use .pug
You need to take the genres input from the frontend and learn how to turn it into an array on the backend. Separate it by commas ( , ) Drama, Comedy, Accion -> ["Drama", "Comedy", "Action"]
Not allowed to type the array from the frontend.
```
