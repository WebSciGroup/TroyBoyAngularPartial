# TroyBoy RPI Marketplace - *Divya, Jialin, Ayah, Chloe*
4/27/2022

Goal: To create a functioning marketplace where students 
can buy and sell goods within rpi domain.

## Roles:

**Divya**: Work on the OAuth login

**Jialin**: Work on homepage and backend
  - SearchBar: Searching keyword in items' titles using MongoDB's query function
  - Filter: Filtering by *condition* and *category* using MongoDB's query function
  - APIs:
    - GET: fetch corresponding items(filter, search bar)
    - POST: add a new item to the database(when users create a new listing)

**Ayah**: Work on the chat api and frontend

**Chloe**: Work on the profile component and backend

## Installation Instructions:

**Backend**:

npm install

npm install typings -g, 
typings install dt~jquery --global --save, 
npm install --save jquery

**Frontend**: 

in the tsconfig.spec.json file add "jquery" to typings[], 

in the tsconfig.app.json file add "jquery" to typings[]

##  Portions where got stuck:

Chloe

With my implemetation of the profile page and a portion of the backend server.js code I
had a lot of difficulty getting the json that I was pulling from my db to connect to the
frontend. For some reason it was working on postman at first,  but I could not get it to 
correctly parse into the frontend. I had to rework a lot of my code on this, and I left 
some of it commented out in the server.js file so you could try to see what the initial
approach was. I also have some commented out code on my profile.ts file because I usually
try to leave an idea of how I initially tried to approach the problems. With jialins help I was able
to take a portion of my code and put some of it into a similar formatting of how she worked using
the http service to connect the frontend with the backend. This ended up working with my api endpoints
for postman and the application. I also had a few errors with how I was intially updating the info
on the profile page. The typescript was not correctly populating the page with the data that I wanted,
so I had to resort to finding some ways that angular can specifically edit html elements. see the profile.html and .ts
files. Now all of that portion of code is working and the last to touch up is some finishing css to match the theme better.

Divya

There were serious issues committing to Github and the login woudn't push with the rest of the files to Github. I completely redid the Oauth again from scratch yesterday by creating a new project in Angular and even then continued to run into technical difficulties today as well.


Ayah

For the comet chat api we ran into a couple issues pushing the code into one repo. We found issue with how the comet chat adata was stored due to the length of the file names and the file path. This caused our github to error multiple times, and despite working with multiple groupmates and teammembers we couldnt get it all into this repo. However, all of the chat is functional and supports many different features such as video call, image upload, and file upload. It worked by creating keys for all of hte users, and all of the data between chats is stored as well. Despite the trouble with github this portion of our porjject is fully implemented and working, as well as the bootstrap and css used to create the interface for troyboy marketplace.

