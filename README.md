# webdev-final-project

## Hi, Welcome to MusicFan

Here is the first version of the project description. Website Link: [to be continued]

## Team Introduction

Development Process: Agile Development

Committing way: feature branch workflow by committing branches and submit pull requests to have code reviewed and committed to the master branch

- Yiwen Sun: [github link here]
- Yu Tang
- Jiayao Li
## Problem Solved

- Problem description

  This is a music application for Apple community that supports music lovers to share and search music. Users can publish their music, edit and delete their post and explore things by different categories.

- Target Users

  - Artist
    - goal 1: create, login and edit profile page
    - goal 2: publish, edit, delete music, search posted history
  - customer
    - goal 1: create and login personal account
    - goal 2: search and add favourite music to his/her playlist, follow other users

## Stategy

#### Font-end

- Tech: React, CSS, JavaScript
  - Login: Google Sign-In API
  - Navbar: React-Bootstrap API
- Implementation
  - Home Page
    - About: a page that explains our mission and design of the site
    - Sign in with Google 
  - Search page
    - search by input text: a page for exploring music to listen by different categories (type in auto-fill: ad-...)
    - search by categories: select certain music type
  - Detail page
    - listed music: title, album, category, length
  - Profile page
    - personal information, playlist, liked songs
    - Publish: authenticated user may enter music description, category and item image url when adding a new post 
    - History: posted songs

#### Back-end

- Tech: Node.js, Express, MongoDB
  - Backend business logic: Node.js
  - Server: Express
  - Database: MongoDB
- Implementation
  - Model
    - Post {title, artist, track name, album, category, length, img url}
    - Post can be edit, delete, add
  - User
    - Account info from Google Sign in API
    - User can sign in and out

#### Test Strategy Design

- Plan for testing content: document specific testing rules based on app features, covering technical reviews, database review, development testing, qualification testing, and acceptance testing
- Plan for testing process: test frontend and backend seperately initially and test the intergrated work

## About API

[Apple Services Performance Partners](https://affiliate.itunes.apple.com/resources/)

The API provides content within the iTunes Store and Apple Books Store, including books, movies, podcasts, music, music videos, audiobooks, and TV shows. We retrive the music data, which contains: musicArtist, musicTrack, album, mix, song, and All Music Guide (AMG) IDs. Here are some API examples that we are going to use in our CRUD process:

- To search for a particular artist's music, e.g. Jack Johnson: 

  https://itunes.apple.com/search?term=jack+johnson&entity=music

- Look up all albums for Jack Johnson:
  https://itunes.apple.com/lookup?id=909253&entity=album

- Look up multiple artists by their AMG artist IDs and get each artist’s top 5 albums: 

  https://itunes.apple.com/lookup?amgArtistId=468749,5723&entity=album&limit=5

## Other Info

**Copyright 2021 © Softaware**
