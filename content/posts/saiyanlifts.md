---
title: "Personal Project: Saiyan Lifts Tracker"
date: 2022-12-26T00:39:46Z
draft: false
---

## The Idea

After brainstorming for a while for a project that would be very useful to my day to day life but not overly ambitious, I came up with the idea of a mobile workout tracker. The apps available now are too bloated and overly complicated for my needs, and often quite slow in saving workouts. Because of these issues my friends and I resort to using notes apps to manually write down exercises done, since it is simply faster. However what if we can have this better speed, and also have the better organisation and looks of the apps? This is the premise of the project.

## The Needs

What does this project need to achieve? I defined the MVP to be a product that is better than any other alternative currently. To achieve this, I want the organisation of storing workout cycles->workouts->exercises, with each having a title and date, and the exercises having sets, reps and load. It must be as fast as the notes app, and have a simple to use UI that is both more pleasant and simple than the notes app.

## The Tech Stack

First, with the need for both fast development (this is my Christmas break project) and fast performance, I defaulted to React for the frontend. For the backend, having learnt postgreSQL extensively at university just last term, I found Supabase which offers a great interface for a postgreSQL database with a free tier more than enough for my needs. With some great advice from my friend Edvins (check out his blog edvins.io!), I found that Next.js is much faster than just using vanilla React, providing a shortcut in the development process. For deployment, Vercel is the best free option by far, with CD from the github repository and database set up in less than 5 minutes. Overall, this combo of Next, Supabase and Vercel is by far the fastest possible trio to get a full stack site up and running for free.

## The Learning

After initialising a create-next-app I started with the Supabase database and authentication quickstart. They have a useful follow along video here: https://www.youtube.com/watch?v=0Fs96oZ4se0. This helped me get familiar with the structure of Next.js and the features provided by Supabase very quickly. Afterwards I took inspiration from this blog: https://blog.logrocket.com/build-full-stack-app-next-js-supabase/#implementing-workout-functionalities, which is an existing workout tracker. It helped substantially to see examples of how things can be done in Next.js, especially with the client-side vs server-side rendering that Next.js does, routing and getting the session effectively everywhere I needed was a challenge initially. Now that I understand it properly though, I find Next.js to be so much faster to set up than vanilla React, with much less work done by the developer to setup routes and the overall architecture of the site.

## The Style

To create an interface more pleasant and simple than the notes app, I opted to have a fixed header and footer design to mimic an app, and used themes from Dragon Ball Z (Broly) to gamify the UI and give the PWA a more polished look. Everything is rectangular apart from buttons, giving it a practical look among the fun theme. Overall I tried to make it look as similar to an app as possible, steering away from awkward browser UI such as popups and complex forms.

## The Journey

27/12/22:
As of now, I have developed above the MVP of the app which I am confident is better than using the notes app to track my workouts finishing with around ~20-30 hours of work in total. What could be added later are a bunch of quality of life features, such as offline compatibility for if I have no signal, and UI improvements in the workout forms to further reduce the actions needed to be performed to log exercises.

Thanks for reading, and I hope you will sign up and enjoy using Saiyan Lifts Tracker as much as I do.

Site: https://saiyan-lifts-tracker.vercel.app/  
Repo: https://github.com/Cheuktingchan/workout_tracker/
