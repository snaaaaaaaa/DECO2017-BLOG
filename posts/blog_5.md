---
title: Blog 5
date: 2026-05-14
author: Sanjana Dommatmari
summary: Prototype Development & Testing Considerations
tags:
  - WACG Criteria
  - User Testing (Think-Aloud Protocol, System Usability Surveys)
---

Having designed the structure of our data and the stand-out feature, we began to thoroughly begin the development process of our prototype in code. 

We decided to begin by first developing the core stand-out feature, the recipe-creation feature. Then we will move on to the browse recipes page and home page, and later to the sub-communities page, as well as any additional features we wish to add to our site if time permits, leaving time for debugging, accessibility checks and UI improvements. I believe it is especially important to structure the progress in this way, as it allows us to prioritise the core features of our prototype (recipe creator, recipe pages, browse page, home page) and ensure their functionality first, before moving on to less-essential or non-essential pages or features. 

This notably applies to the user-created sub-communities page, as at this stage it may largely be static elements with some dynamic components, but detached from a database. While I still feel the communities page is an important contributor to our web app’s purpose in serving the needs of home cooks, I acknowledge that it may be outside of the scope of this assignment to thoroughly build out this page. The feasibility of this page will be determined in a later stage of development. Hence, at this stage, a trade-off may be to leave the communities page as a future addition, and instead flesh out the existing core pages with more features (ability to save recipes, a simple saved recipes page/section, etc.). 

To develop the recipe-creation feature while following a modular design philosophy, I have been developing it as its own component, which is rendered with the user profile page template. I am currently developing it as an on-page element, to first ensure functionality, however I intend its final form to be an overlay panel which appears on the profile page after a button is pressed. Developing it as a component in this way allows me to be flexible with how it is implemented, and make localised changes which do not affect the rest of the page. 

Moreover, the design system will be finalised after the key components are functioning as intended. During the finalisation and implementation of this system, it is essential to check the design and overall web app against Web Content Accessibility Guidelines (WACG), to ensure accessibility needs are thoroughly met. For our prototype, the most prevalent criteria will likely pertain to colour contrast, text handling, and user navigation. 

Additionally, in this sprint I realised the need to revisit the user flow of the prototype. While I planned the user flow and site structure of the website a few weeks ago, now that the structure of the core feature has been finalised, this flow will need to be revisited for clarity and usability. Specifically, user testing should be conducted with our built prototype with home cooks within the user base,  to ensure that the key features of our prototype are understood by the users without additional documentation or instruction required. These tests can be conducted using the Think-Aloud-Protocol, to record pain points and areas of success, as well as a System Usability Survey (SUS) to gather overall quantitative testing data. 
