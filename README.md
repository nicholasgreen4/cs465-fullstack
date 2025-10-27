# cs465-fullstack
Travlr Getaway Full Stack Web Application

## Architecture

Compare and contrast the types of frontend development you used in your full stack project, including Express HTML, JavaScript, and the single-page application (SPA).
Why did the backend use a NoSQL MongoDB database?

  This project used two different frontend development techniques: Express HTML and JavaScript for the customer-facing site, and an Angular Single-Page Application (SPA) for the administrative dashboard. The Express-based frontend uses Handlebars templates to render HTML pages directly from the MongoDB serve. This approach offers a simple web browsing experience--each page request triggers a new server call and reloads the browser view; the server controls rendering and content delivery. The Admin portal, in contrast, uses an Angular SPA which provides a more interactive and dynamic user experience. The SPA handles page routing, data management, and user interface. Once loaded, the SPA communicates with the database using HTTP requests and updates the view without needing the browser page to be reloaded.
  The backend for this project uses a NoSQL MongoDB database because it provides a flexible structure, allowing for dynamic data models. This is beneficial in a travel booking application where the data being stored, such as travel packages, destinations, etc, may vary significantly. 

## Functionality

How is JSON different from Javascript and how does JSON tie together the frontend and backend development pieces?
Provide instances in the full stack process when you refactored code to improve functionality and efficiencies, and name the benefits that come from reusable user interface (UI) components.

  JSON stands for JavaScript Object Notation; it is a lightweight data format used for storing and exchanging data between (in this case) the frontend and backend. JavaScript is a complete programming language used to create functional, interactive web applications.
  Throughout developement, several pieces of code were refactored. For example, route handlers in Express were split into separate modular files to simplify maintenance and prevent redundancy. In the Angular SPA, reusable UI components were implemented to standardize the appearance and behavior of the application. Refactoring the code into a more modular structure like this made scaling the project easier and allowed for easier maintenance. 

## Testing

Methods for request and retrieval necessitate various types of API testing of endpoints, in addition to the difficulties of testing with added layers of security. Explain your understanding of methods, endpoints, and security in a full stack application.

  Testing in a full-stack environment requires validating multiple levels of the program. RESTful API testing focuses on methods like: GET, which retrieves existing data, POST, which creates new data, PUT/PATCH, which updates existing data, and DELETE, which removes data. Beyond that, each endpoint must be tested to ensure proper responsiveness, error handling, and integrity. 
  Security testing requires ensuring that protected endpoints require necessary authentication and that such authorization cannot be easily bypassed.
