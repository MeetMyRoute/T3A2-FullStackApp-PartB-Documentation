# T3A2: Full Stack App (Part B) Documentation

## MeetMyRoute

### Links

* [Deployed Front-End]()  
* [Deployed Back-End]()
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