# T3A2: Full Stack App (Part B) Documentation

## MeetMyRoute

### Links

* [Deployed Front-End](https://meetmyroute.netlify.app/)  
* [Deployed Back-End](https://meetmyroute-api.onrender.com)
* [GitHub Front-End Repository](https://github.com/MeetMyRoute/T3A2-FullStackApp-PartB-FrontEnd)  
* [GitHub Back-End Repository](https://github.com/MeetMyRoute/T3A2-FullStackApp-PartB-BackEnd)
* [Part A README](https://github.com/MeetMyRoute/T3A2-FullStackApp-PartA)  
* [Trello Board](https://trello.com/b/ay0VQxw7/t3a2-full-stack-app)  

### Libraries & Dependencies

#### Back-End

* `bcryptjs` - Used to hash passwords before storing it in the database to ensures sensitive data like passwords are secure
* `cors` - Used to enable or restrict the different origin/domains that can interact with the back-end API server
* `dotenv` - Used to load environment variables from a `.env` file so ensure that sensitive data like database URIs remain protected
* `express` - Used to build the back-end API and handle HTTP requests
* `express-async-handler` - Used to automatically handle errors in async routes in ExpressJS
* `jsonwebtoken` - Used to generate and verify JWT tokens
* `mongodb` - Used to establish a connection and perform CRUD operations with the MongoDB database
* `mongoose` - Used for data validation, schema creation and model definition for the MongoDB database
* `nodemailer` - Used to send email notifications from NodeJS apps like password reset
* `nodemon` - Used to automatically restart the Node apps when changes are detected during development

#### Front-End

* `axios` - Used to make Promise-based HTTP requests from the front-end and supports async/await usage
* `date-fns` - Used to manipulate and format JS dates
* `dotenv` - Used to load environment variables from a `.env` file so ensure that sensitive data like API URLs remain protected
* `react` - Used for building user interfaces
* `react-datepicker` - Used for data selection in a calendar format
* `react-dom` - Used to render React components and serves as the entry point to the DOM
* `react-router-dom` - Used to handle routing in React apps
* `vite ` - Used to improve the development experience of building user interfaces

### Source Control Methodology
We used GitHub to manage all source control. The project was organised into two separate repositories: one for the front-end and one for the back-end. A new branch was created for each feature and once the feature was completed, it was merged into the main branch to ensure a clean and manageable codebase.

<details>
<summary>GitHub Screenshots</summary>

#### Repositories
![GitHub Repos](./docs/github-repos.png)  

#### Back-End Branches
![GitHub BE Branches](./docs/github-be-branch.png)  

#### Front-End Branches
![GitHub FE Branches](./docs/github-fe-branch.png)  

</details>

### Project Management & Task Delegation
We used Discord as our primary platform for communication and Trello for tracking progress. The To-Do list on Trello was organised into Front-End and Back-End tasks. Each card was labelled to identify which feature the task related to and checklists were added to monitor progress and track the remaining steps required to complete each task.

We decided to delegate tasks based on features, ensuring that all team members gained hands-on experience in both front-end and back-end development for their assigned features. This approach helped promote a well-rounded understanding of the entire project and allowed for efficient collaboration.

<details>
<summary>Trello Board Screenshots</summary>

#### 28.11
![Trello](./docs/trello-28.11.png)   

#### 30.11
![Trello](./docs/trello-30.11.png) 

#### 2.12
![Trello](./docs/trello-2.12.png)   

#### 3.12
![Trello](./docs/trello-3.12.png)   

#### 6.12
![Trello](./docs/trello-6.12.png)   

#### 7.12
![Trello](./docs/trello-7.12.png)   

#### 8.12
![Trello](./docs/trello-8.12.png)

#### 13.12
![Trello](./docs/trello-13.12.png) 

#### 22.12
![Trello](./docs/trello-22.12.png)    

</details>

## Part A Documentation

### Purpose

This application is designed to connect travelers with others who share similar travel interests or itineraries, whether they are fellow travelers or locals in their desination area. It aims to create a platform where travelers can find companionship, receive local insights, or even arrange meetups to enhance their travel experiences. By faciliating these connections, the app helps travelers feel more secure, get personalised travel tips, and enjoy shared experiences, especially those traveling alone.

### Functionality/Features

* User profiles:
    * Users create a profile where they share personal travel interests and bio information.
    * This profile is visible to others.
    * Users can set their profile status to either "Private", "Traveling", or "Local".

* Shared and private itinerary:
    * Users share upcoming travel plans by entering their destination(s) and travel dates.
    * Users add other trip information that are not shared publicly.

* Search and filtering:
    * Users can explore the community by searching for travelers with overlapping itineraries.
    * The app will have filters such as destination and date.

* Real-time chat and messaging:
    * A built-in chat feature allows users to connect and discuss plans, ask questions, or arrange meetups.

### Target Audience

The application is designed for all travelers but is particularly beneficial for solo travelers, who may seek companionship, security, or local guidance to enhance their journeys.

### Tech Stack

* Front-end
    * HTML
    * CSS
    * Javascript
    * React

* Back-end
    * Express
    * Node.js
    * Mongoose

* Database
    * MongoDB

* Deployment
    * Netlify - front end
    * Render - back end

* Project Management
    * Trello

* Diagramming
    * Draw.io

* Design
    * Figma

* DevOps
    * Visual Studio Code
    * Git
    * GitHub

### Competitor Research

We've identified two primary competitors in the travel companion space and took inpiration from: NomadHer and TripBFF.

* NomadHer
    * Target audience - female travelers.
    * Key features:
        * Community-focused - sharing stories and tips.
        * Social networking - connecting with like-minded individuals.
        * Travel buddy matching - finding companions with similar itineraries.

While we appreciated the community of NomadHer, we decided to make our app open to all travelers rather than focusing solely on one demographic. Additionally, although sharing stories and tips publicly is a valuable feature, we decided it was outside the scope of our project.

* TripBFF
    * Target audience - general travelers.
    * Key features:
        * Collaborative trip planning - creating and sharing itineraries.
        * Travel tips and advice - accessing expert insights.
        * Destination discovery - exploring new places.
        * Nearby traveler discovery - connecting with local travelers.
        * Travel tracking - monitoring progress and sharing experiences.
        * AI-powered trip planning - leveraging AI for personalised recommendations.

TripBFF, while it offers many features, one major differentiator is that TripBFF does not allow users to filter by travel dates, which our app will offer as a key advantage. This ability to search and filter by specific dates helps users find matches more precisely, making it easier to connect with others whose itineraries overlap.

In terms of design, both NomadHer and TripBFF feature light, clean interfaces with a dominant colour. We aim to maintain this minimalist approach in our app's design. While blue is a common choice for travel apps, symbolising trust and freedom, we opted for sunset orange to evoke warmth, excitement, and the thrill of exploration, aligning with the core values of our app.

### Dataflow Diagram
![Dataflow Diagram](./docs/dataflow-diagram.png)

### Application Architecture Diagram
![Application Architecture Diagram](./docs/application-architecture-diagram.png)

### User Stories 
--- 

![Jessica Turner](./docs/user1.png)  
**Jessica Turner**

**Role**: Photographer and Journalist  
**Location**: London, United Kingdom

**Background**: 
Jessica has spent over a decade as a photographer and journalist, using her lens and words to tell captivating stories from across the globe. Her deep love for photography and storytelling has inspired her to start a travel blog, where she plans to share her adventures and highlight the journeys of other travellers she meets along the way. Jessica's ultimate goal is to connect with fellow globetrotters and create a community of travellers who share their experiences, photos, and travel tips through her blog.

**Goals**: 
- Find like-minded travelers to interview and photograph for her blog. She seeks to build a network of travelers to connect with.
- Feature diverse voices in her blog by telling stories from people with varying travel itineraries. 
- Simplify her content creation process by quickly finding collaborators, getting their stories, and capturing unique images on the go. 

**Challenges**: 
- Difficulty in Connecting with Like-minded Travelers:  
  Jessica has a niche audience and often finds it challenging to connect with travelers whose journeys align with her unique itineraries.

- Managing Multiple Platforms:  
  Juggling various social media and travel platforms can be overwhelming. Jessica is looking for a more streamlined way to find the right people for her blog, without the hassle of using multiple platforms.

- Time Constraints:  
  With frequent travels, Jessica needs quick and efficient solutions to identify potential blog collaborators without investing too much time.

---
**Why MeetMyRoute**:  
- Familiar Interface:  
  Jessica downloaded MeetMyRoute because its interface reminded her of the dating apps she was already familiar with, making it both easy and intuitive to navigate.

- Simple Search & Discovery:  
  The app’s search functionality lets Jessica filter travelers by destination and travel dates, making it easier to find the perfect subjects for her blog and photography projects.

- Simplified Communication:  
  Meet My Route’s real-time messaging feature allows Jessica to arrange photography sessions and collaborate directly with travelers, eliminating the need for third-party communication tools.

--- 
![Josh Smith](./docs/user2.png)  
**Josh Smith**

**Role**: University Student  
**Location**: Manchester, United Kingdom

**Background**: 
Josh has recently taken a gap year from university to explore the world before returning to his studies. This is his first time traveling internationally, and he’s eager to embrace new cultures and experiences. With enough savings to embark on a backpacking adventure, Josh plans to visit multiple countries throughout the year, looking for authentic experiences and opportunities to meet other travelers. His primary goal is to gain valuable insights into the cities and cultures he visits, learning from those who have traveled more extensively. He seeks to connect with more experienced travelers for advice, recommendations, and even potential travel companions.

**Goals**: 
- Connect with like-minded travelers to share experiences and travel advice, building a network of fellow backpackers along the way.
- Use a simple, intuitive app that makes it easy to find and connect with fellow travelers, without overwhelming features or complicated navigation.
- Find trustworthy travel companions for shared adventures and group activities, ensuring safety and mutual enjoyment.

**Challenges**: 
- Navigating New Destinations Without Local Knowledge:  
  Since Josh is new to traveling, he may struggle with finding local tips, hidden gems, or travel advice while in a new city. He wants to connect with experienced travellers who can share valuable recommendations and insights for exploring the area.

- Overwhelmed by Complex Apps:  
  Josh dislikes apps that are hard to navigate or have too many unnecessary features. He needs something easy to use without spending too much time figuring out how to operate it.

**Why MeetMyRoute**: 
- Recommended by a Friend:    
  Josh discovered the app through a recommendation from someone he met at a bike store. 

- User-Friendly Interface:   
  Josh can create a profile and plan his trip with MeetMyRoute’s simple, user-friendly layout, establishing his goals for the trip. The app allows him to easily connect with other travelers, without overwhelming him with complex features.

- Curated Itineraries with Like-Minded Travelers:  
  Josh finds other travellers who have similar hobbies and travel intentions thanks to MeetMyRoute. This makes it simple for him to find undiscovered treasures and distinctive experiences that suit his preferences.

--- 
## User Story 1: Profile Creation
```md 
As Jessica,
I want to create a profile on the app, 
So that I can establish myself as a blog writer and photographer, and attract potential collaborators.
```
**Acceptance Criteria**: 
- The profile creation form should gather basic information such name, location, travel preferences, and goals. 
- Users should be able to upload a profile picture.
- Validation should be included in the form to guarantee that all required fields are filled out.
- Users should be taken to their profile page to view and modify their information after submitting.

```md
As Josh,  
I want to create a profile on the app,  
So that I can establish myself as an emerging traveler and seek insights from more experienced travelers. 
```
**Acceptance Criteria**: 
- For broader networking, users should be able to link their social media profiles on the form.
- Before submitting, users should be able to view their profiles on the system.
- The profile is active after submission, and the user may update their details at any time.

## User Story 2: Connecting with Other Travelers
```md
As Jessica,
I want to connect with other travelers who have similar itineraries,
So that I can collaborate with them for blog content and photography projects.
```
**Acceptance Criteria**: 
- Users should be able to search for travelers with overlapping itineraries using filters like destination and travel dates.
- The system should display traveler profiles that match the selected filters.

```md
As Josh,
I want to search for travelers who are heading to destinations I’m interested in,
So that I can join their adventures. 
``` 
**Acceptance Criteria**: 
- Users should be able to use a search bar to find travelers. 
- After searching for travelers, users should be able to view the profile status of each traveler (e.g., 'Travelling,' 'Local,' or 'Private') to understand who is currently traveling. 

## User Story 3: Messaging for Collaboration

```md
As Jessica,
I want to communicate directly with fellow travelers through the app's messaging feature,
So that I can arrange collaborations for interviews and photography sessions without needing third-party apps. 
```

```md
As Josh,
I want to communicate with other travelers directly through the app,
So that I can discuss travel routes, find a travel buddy, and get recommendations for affordable places to stay.
```

**Acceptance Criteria**: 
- Users should be able to send files (documents, images, etc.) and view earlier chats.
- Users should be able to send direct messages through the platform, opening in a separate window for a cleaner interface.
- Notifications should be sent to users when they receive messages.

## User Story 4: Itinerary Management

```md
As Jessica,
I want to create and manage my travel itinerary on the app,
So that I can plan my trips and connect with others who have similar travel goals.
```

**Acceptance Criteria**: 
- Users should be able to enter dates, travel destinations, and key activities for each trip using the app. 
- Itineraries should be customisable by adding or removing destinations, dates, and activities.

```md
As Josh,
I want to organise my trips in the itinerary feature,
So that I can easily keep track of my travel plans and control who can see them.
```

**Acceptance Criteria**: 
- Users should be able to update specific travel dates and times for planned destinations. 
- Users should be able to toggle between a detailed itinerary (dates, destinations, activities) and a simplified itinerary (dates, destinations), and share/view other's simplified itineraries.

### Revision and Refinement:

After engaging with users, we identified privacy concerns regarding the public sharing of detailed itinerary information. While users were open to sharing relevant details, they expressed the need for greater control over what components of their itinerary are visible to others.
Initially, we considered incorporating a toggle feature to allow users to switch between a detailed list and a simplified view of their itinerary for a more flexible experience. However, following user feedback, we recognised the importance of addressing concerns about sharing additional information, such as activities, publicly. This feedback reinforced the need to give users more discretion over the visibility of their itinerary details.

Based on this input, we have decided to implement the following:
- The simplified itinerary view, which includes only dates and destinations, will be publicly shareable.
- The detailed itinerary, containing more comprehensive information, will be private to the user. 

Users can securely share additional details, including accommodations, through direct messages, ensuring their privacy concerns are addressed. 

### Wireframes

#### Desktop View
![Desktop View](./docs/desktop-view.png)

#### Tablet View
![Tablet View](./docs/tablet-view.png)

#### Mobile View
![Mobile View](./docs/mobile-view.png)

#### Overview
The wireframes developed for this application represent three standard sizes: Desktop, Tablet and Mobile View.

* Home Page
  * This page introduces the app.
  * The layout is responsive - on desktop view, the text is positioned to the left and the image is positioned to the right, while on tablet and mobile view, the layout switches to a single-column layout.
  * The Login and Sign Up buttons redirects the user to the Login and Sign Up page respectively.

* Sign Up Page
  * This page allows new users to register for the app.
  * The layout is response - on desktop view, the email and password fields are positioned to the left and the name. location, status (dropdown), travel preferences and goals and link to social media fields are positioned to the right, while on tablet and mobile view, the layout switches to a single-column layout.
  * The Sign Up button redirects the user to the Profile page once registration is completed and the Login button redirects the user to the Login page.

* Login Page
  * This page allows returning users to log into the app.
  * The layout is consistent across all screen sizes.
  * The Login button redirects the user to the Profile page once the user has logged in successfully and the Sign Up button redirects the user to the Sign Up page.

* Profile Page
  * This page allows users to view and manage their own profile, with a similar layout when viewing other viewing other users' profile.
  * The layout is responsive - on desktop view, the profile information is displayed in a two-column format and is split with name, location, profile picture and status positioned on the left and the remaining fields on the right, while on tablet and mobile view, the layout switches to a single=column format and the navbar (on this page and all following pages) is condensed into a sidebar to maximise on spacing.
  * The Edit Profile button is shown when viewing the user's own profile and changes to a Message button when viewing another user's profile.
  * The Message button redircts the user to the Message page.

* Itinerary Page (View List)
  * This page allows users to view and manage their itinerary lists.
  * The layout is responsive - on desktop view, the itinerary sections are displayed in a two-column format, while on tablet and mobile view, the layout switches to a single-column format.
  * The Edit Itinerary button will redirect the user to the Itinerary (Add/Edit New Itinerary) page.

* Itinerary Page (Add/Edit New Itinerary)
  * The page allows users to add a new or edit an existing itinerary.
  * The Submit button is shown when adding a new itinerary and changes to an Update button when editing an existing itinerary.
  * The layout is consistent across all screen sizes.
  * The Submit and Update button redirects the user to the Itinerary (View List) page.

* Message Page
  * This page allows users to view, send and delete messages.
  * The layout is responsive - on desktop view, the messages are displayed in a two-column format with the list of conversations (the other user's name displayed) on the left and selected conversation messages on the right, while on tablet and mobile view, the layout switches to a single-column format with the selected conversation showing a sidebar to allow users to go back and view the conversations list.

* Search Page
  * This page allows users to search for other users based on destination, travel dates and status.
  * The layout is responsive - on desktop view, the filters and results are displayed in a three-column format, while on tablet view, the layout switches to a two-column format and on mobile view, the layout switches to a single-column layout.
  * The View Profile button redirects user to the Profile page.

### Trello Board

We utilised a Trello board to effectively track our progress throughout the project. Tasks necessary to complete this part of the assignment were added to the board and assigned based on individual preferences and areas of interest.

During the project, we leveraged Trello's built-in features, such as due dates and checklists, to stay organised and maintain steady progress. These tools helped us break down the work into manageable pieces and monitor our workflow efficiently.

We adopted an Agile methodoloty to ensure iterative improvement and collaboration. This approach is evident in screenshots dated 14.11.24, 15.11.24, and 17.11.24, where the card Part A: Description of the Website was reviewed after its initial development, refined through subsequenet iterations, and finally approved upon completion. This iterative procress allowed us to adapt and improve the deliverable based on feedback and evolving requirements.

<details>
<summary>Screenshots</summary>

#### 12.11.24
![Trello Screenshot](./docs/trello-12.11.png)

#### 13.11.24
![Trello Screenshot](./docs/trello-13.11.png)

#### 14.11.24
![Trello Screenshot](./docs/trello-14.11.png)

#### 15.11.24
![Trello Screenshot](./docs/trello-15.11.png)

#### 17.11.24
![Trello Screenshot](./docs/trello-17.11.png)

#### 18.11.24
![Trello Screenshot](./docs/trello-18.11.png)

#### 20.11.24
![Trello Screenshot](./docs/trello-20.11.png)

#### 24.11.24
![Trello Screenshot](./docs/trello-24.11.png)
![Trello Screenshot](./docs/trello-24.11-2.png)
![Trello Screenshot](./docs/trello-24.11-3.png)

</details>
