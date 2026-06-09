---
title: A3 Reflection 
date: 2026-06-09
author: Sanjana Dommatmari
summary: My final reflection of our community web app prototype, evaluating its performance, user experience, the development of functional requirements, and a reflection on lessons learned.
tags:
  - Final Reflection
  - Evaluation
  - Performance
  - User Testing
  - Think-Aloud Protocol
  - Functional Requirements
---
After now having completed our prototype, I believe we were successful in making a tailor-made community web app for home cooks. Though there were many hurdles faced along the way, such as the actual development process, reevaluating design decisions, and the technicalities of working collaboratively, overall we were able to distill a broad idea into core tangible, and functional features. 

<h2>Performance:</h2>

On the whole, the prototype performs efficiently and reliably throughout the different pages. All prototyped interactions work as intended and with fast load times. As well as this, throughout user testing, all buttons, hover features, type features, form submissions, and image loading responded reliably. 

In terms of error handling,  development of the prototype, I found that it was important to ensure the front-end javascript file for the serving scaler loaded properly, as it existed outside of the MVC structure the majority of the site is developed in. This test can be seen in the console with a debug log, ensuring the serving scaler is loaded, as well as the number of elements it recognises in the ingredients list which can be scaled.

![Serving Scaler non-active](assets/serving-scaler_home.png) 

<i>Figure 1: Screenshot of console Home Page</i>

![Serving Scaler Active](assets/serving-scaler_recipe.png) 

<i>Figure 2: Screenshot of console on Recipe Detail page, detecing the serving scaler</i>

In order to further evaluate the performance of our prototype, I ran a lighthouse audit on the different main pages of the site, where the results of the audits can be seen in the screenshots below. 

![Home page lighthouse audit](assets/lighthouse_home.png) 

<i>Figure 3: Screenshot of Lighthouse audit for the Home Page</i>

![Browse page lighthouse audit](assets/lighthouse_browse.png) 

<i>Figure 4: Screenshot of Lighthouse audit for the Browse Page</i>

![Communities page lighthouse audit](assets/lighthouse_communities.png) 

<i>Figure 5: Screenshot of Lighthouse audit for the Communities Page</i>

![Profile page lighthouse audit](assets/lighthouse_profile.png) 

<i>Figure 6: Screenshot of Lighthouse audit for the Profile Page</i>

![Recipe page lighthouse audit](assets/lighthouse_recipe.png) 

<i>Figure 7: Screenshot of Lighthouse audit for a Recipe Detail Page</i>

 
As evident in the results of these audits, our prototype performs well, with high performance scores, and load times consistently under one second. 

The following four criteria were identified as consistent areas for improvement: 
- Improve image delivery 
- Render blocking requests 
- Use efficient cache lifetimes 
- LCP request discovery 

A majority of these criteria are largely a result of this prototype being my group’s first experience developing a dynamic web app, and in the future can be resolved through better practices and techniques to improve load times. With this said, the ‘Improve Image Delivery” criteria appears to be a direct result of our attempts to have high-quality images throughout our site, as the aesthetic of the pictures are fundamental to the experience of our prototype. In the future, we would work to implement relative sizing, or use other image formats to improve image download speeds. 

<h2>User Experience:</h2>

The user experience of our prototype was thoroughly considered throughout development, to create an accessible online space which promoted enjoyment and return engagement with the web app, while also delivering a tailor-made experience for home cooks. Overall, I believe we were quite successful in achieving this intended user experience through our various design choices. These include:
- A clean, high-contrast, semi-minimalist design 
- A limited colour palette with a clear primary and secondary colour to achieve visual cohesion throughout the site 
- Card & section-based layout for increased readability
- Clear text hierarchy to differentiate page sections and features
- Sans serif font for easy readability 
- Subtle hover state animation and colour states to increase affordance

As well as this, we also prioritised the accessibility of our site, by checking it against relevant WCAG AA criteria. Through these checks, we ensured that the site is entirely accessible through keyboard navigation, all images have alt text, elements on the page have a suitable level of visual contrast, reflow content can be presented without a loss of information or functionality, and that text is appropriately spaced apart. The thorough accessibility of our site is also supported by the results of the lighthouse audits seen in figures 3-7 above. 

Moreover, in order to ground these observations in evidence, I conducted user testing with two participants using a Think-Aloud Protocol. In this testing, I asked participants to complete a set of four tasks, while taking notes on their behaviour and verbal protocol, as seen in the tables below. 

![User Testing part 1](assets/user-testing_1.png) 
![User Testing part 2](assets/user-testing_2.png) 
![User Testing part 3](assets/user-testing_3.png) 

The testing hence supported the usability of our prototype, as users were able to complete all tasks quickly and efficiently, without any extra required guidance or prompting.

With this said, the testing revealed a few minor improvements which could be made to improve the clarity of interactions
- Like button: One user was slightly confused by the nomenclature of the ‘Likes’ button. This can be fixed by replacing it with a thumbs up icon, which adheres more to convention
- Create recipe button: One user hesitated when trying to locate the ‘Create Recipe’ button, as they were confused as to which page it would be located on. This could be amended by making it a universal feature in the nav bar, or adding additional informational text which leads users to the profile page. 


<h2>Functional Requirements:</h2>

Overall, we were able to meet the key, high priority features established during the planning phase. However, our original scope was too large, and we had to reevaluate, as well as entirely cut a couple of features throughout the process. 

<h3>Developed to original scope:</h3>

I believe a crucial part of our prototype’s success was pioritising the development of core features, and ensuring their functionality above others in order to maintain the scope. These include the main pages (home, browse recipes, community, profile) and key features, including browsing and filtering through recipes, and our recipe creation stand-out feature.

<h3>Rescoped throughout development:</h3>

Though some features had to be rescoped, we adapted them to ensure their purpose was still properly represented. 

<u>Recipe Comments & Adaptations:</u>
We initially intended to have unique comments and adaptations for each recipe, however the data handling required is beyond the scope of this prototype. In order to keep the features, we developed them as generic partials and loaded the same example posts into every recipe page, instead of linking unique posts to recipe data. This ensured we could still showcase these key features, ensure they’re functioning, while remaining within scope.

<u>Community page & features:</u>
While we developed a working ‘Join Community’ button, to remain within scope we only built out one community page with a static layout. In a fully-built product, all the features on the page would be functional, and each community page would have a similar structure.

<h3>Cut features for future development:</h3>

Some features had to be cut from our prototype due to feasibility, but would ideally be included in a future, fully developed web app.

<u>Converting ingredient lists to shopping lists:</u>
This feature was intended to connect ingredient lists to shopping lists connected to real supermarkets. However, it would have involved complex external integration, and was outside the scope of this project.

<u>Saving recipes:</u>
This feature would allow users to save recipes, which would appear on their profile page. It was cut due to feasibility, and to prioritise the development other key features,

Hence, though our initial scope was too large, as we were able to rescale many of our features and fully develop our core functionalities, I believe our goals were fairly realistic, and that we were successful in creating a tailor-made experience for home cooks. 



<h2>Lessons Learned:</h2>

Overall, the development of this prototype was a significant learning process. Firstly, as I had never worked with dynamic websites, I found it a challenging subject to thoroughly grasp. Particularly, routing, and understanding the MVC structure of the project and how it interacts with persistent data was a notable hurdle in the development process. However, having finished development, I now have a much better grasp of how good web design decisions begin in the foundations of the back-end, and then translate visually to the front-end. 

Moreover, another challenge was learning how to collaborate using Github. It was fundamental learning how to communicate effectively in order to split tasks amongst us to work on different files, while still making progress and prioritising features throughout. 

What I felt was most significant to my experience of web development, was learning to assess and refine scope as development progresses. As the feasibility of this project was less initially predictable (likely due to my inexperience), the scope had to regularly be reviewed and revised throughout development. This highlighted the importance of regularly assessing feasibility, while also teaching me how to adapt out-of-scope features to be more realistic, while still maintaining their purpose. In turn, I feel that I can now confidently apply this thinking and design approach to future projects, to achieve better-developed results. 


