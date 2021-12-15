
# Project's name
​
Doggy
​
## Description
​
It is an application to be able to meet people who have dogs and to be able to make group outings
​
## USER STORIES
​
**404** - As a user I want to see a nice 404 page when I go to a page that doesn’t exist so that I know it was my fault
​

**500** - As a user I want to see a nice error page when the super team screws it up so that I know that is not my fault
​

**Homepage** - As a user I want to be able to access the homepage so that I see what the app is about and login and signup
​

**Sign up** - As a user I want to sign up on the webpage so that I can see all the events that I could attend
​

**Login** - As a user I want to be able to log in on the webpage so that I can get back to my account
​

**Logout** - As a user I want to be able to log out from the webpage so that I can make sure no one will access my account
​

**Profile** - As a user I want to be able to see my profile and edit it
​

**Add new meeting** - As a user I want to be able to create new meetings with other people
​

**List of meetings** - As a user I want to be able to see my meetings
​

**Delete meeting** - As a user I want to be able to delete my meetings
​

**Update meeting** - As a user I want to be able to update the information of my meetings
​

**Add new dog** - As a user I want to be able to add a new dog.
​

**List of my dogs** - As a user I want to be able to see my dogs.
​

**Delete dog** - As a user I want to be able to delete my dogs.
​

**Update dog** - As a user I want to be able to update the information of my dog.
​

## BACKLOG
​
**Catalog filter** - As a user I want to be able to carry out a meeting search in my area
​

**To be able to join meetups** - As a user I want to be able to join meetups
​

**Record of meetups created** - As a user I want to see the meetings that I have created
​

**Meetings in which I have participated** - As a user I want to see the meetings that I have been
​

## Routes
​
| Name            | Method | Endpoint                      | Description                                      | Body                                  | Redirects       |
| --------------- | ------ | ----------------------------- | ------------------------------------------------ | ------------------------------------- | --------------- |
| Home            | GET    | /                             | See the main page                                |                                       |                 |
| Log in form     | GET    | /login                        | See the form to log in                           |                                       |                 |
| Log in          | POST   | /login                        | Log in the user                                  | {mail, password}                      | /               |
| Sign Up form    | GET    | /signup                       | See the form to sign up                          |                                       |                 |
| Sign Up         | POST   | /signup                       | Sign up a user                                   | {mail, password}                      | /profile        |
| Log out         | GET   | /logout                       | Log out a user                                   |                                       | /               |
| Profile         | GET    | /profile                      | See the profile page with editable form          |                                       |                 |
| Profile edited  | POST   | /profile                      | Send user's data changed                         | {user_email, password                 | /profile}       |
| Garden          | GET    | /garden                       | See user's garden collection                     |                                       |                 |
| Plant           | GET    | /garden/plantid               | Read plant's information                         |                                       |                 |
| Pland add form  | GET    | /garden/new                   | See form to upload a new plant                   |                                       |                 |
| Plant add       | POST   | /garden/new                   | Upload a plant to user's garden                  | {nickname, user_pics, shopping_point} | /garden/plantid |
| Plant edit form | GET    | /garden/plantid/edit          | See edit form with plant's preloaded information |                                       |                 |
| Plant edit      | POST   | /userid/garden/plantid/edit   | Add plant's new information                      | {nickname, user_pics, shopping_point} | /garden/plantid |
| Plant delete    | POST   | /userid/garden/plantid/delete | Delete plant from user's garden                  |                                       | /garden         |
​
## Models
​
User model
​
```js
{
    userEmail: String,
    hashedPassword: String,
    location: Array,
    age: Number,
    img: String,
}
```
Dog model
​
```js
{
    name: String,
    sex: String,
    race: String,
    size: Array,
    age: Number,
    img: String,
}
```
​
Meeting model
​
```js
{
    nameOfUser: String,
    day: Number,
    timeStart: Number,
    timeEnd: Number,
    place: Array,
    imgMaps: String,
}
```
​
​
## Links
​
### Github project
​
[Github project](https://github.com/)
​
### Git
​
URls for the project repo and deploy
[Link Repo](https://github.com/)
[Link Deploy]()
​
### Wireframes
​
[InVision with Wireframes]()
​
### Slides
​
URls for the project presentation (slides)
[Link Slides.com]()
