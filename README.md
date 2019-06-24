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
