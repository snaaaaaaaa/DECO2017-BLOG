---
title: Blog 4
date: 2026-05-11
author: Sanjana Dommatmari
summary: Designing Data
tags:
  - Data Definition Document (DDD)
  - Entity Relationship Diagram
---
This week, we began to design and finalise the structure of our site’s data, and plan how it would be implemented into our site’s features. 

To do this, we first finalised our stand-out feature, what data it will require, and how it will integrate into the overall flow and structure of the website. We decided that our recipe creation feature will have a set format which allows users to easily upload a recipe into a structured form, with a picture, and selecting a range of tags to describe the recipe, as well as making it easier to categorise in the overall browse page. The sketch below illustrates our planning of this feature and its structure.

[RECIPE CREATION FUNCTION NOTEBOOK SKETCH]

Our recipe creator will be accessed through the user’s profile page. After the user submits the completed recipe, it will appear as a recipe card on both their profile page, and the browse recipes page, and clicking on each card will render a template for a dedicated recipe page. These recipe pages will have all the associated steps and ingredients, as well as multiple components as features, such as comments, and community contributed adaptations. 

With our main feature finalised we began to structure our Data Definition Document (DDD). As the nature of our feature leaves large room for variety in the user input, namely in the ingredient names, instructions, and comments, we realised our data would require numerous tables, and so we did multiple passes when creating our DDD to ensure each attribute has only one example value. This left us with five tables for recipes, tags, ingredients, steps and comments, and one junction entity for recipe_tags. We then used ChatGPT to help convert our tables into DBML, where we then put this schema into dbdiagram.io to generate an Entity Relationship Diagram (ERD). 

[ERD SCREENSHOT]

After discussing our DDD with a tutor however, they mentioned that five or six tables is likely the limit of the scope for this type of assignment, and that more complicated data designs may affect the feasibility of our design. Furthermore, if we wish to incorporate community adaptations as well, this will have to be a separate DDD table as well, which widens the scope further. 

To address this concern, for the context of this prototype, I feel that we  may have to consider having these components detached from specific recipes, and instead build them as separate partials which are loaded each time a recipe page is rendered. They will still be dynamic page elements, however instead of being associated with recipe data, they will act as generic stand-ins for how the features would behave in a fully-developed version of the web app. 

Moreover, we also wanted to incorporate an option to turn recipe lists on pages into shopping lists, which link to existing supermarket websites. We believe this could be a key feature which incorporates advertising opportunities, as well as tailor-made experiences as highlighted in the brief. However, considering the scope once again, it may likely only be incorporated as a static or presentation-level element without real links to data for this prototype. 
