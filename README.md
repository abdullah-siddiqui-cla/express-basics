# Exercise 1: Setting Up a Basic Server
## Objective: Create a simple Express server that listens on port 3000.
## Steps:
- Install Express.
- Create a route for the root path (/) that responds with "Welcome to Express!".
- Start the server and verify it works by visiting http://localhost:3000.

# Exercise 2: Adding Multiple Routes
## Objective: Create routes to handle different paths.
## Steps:
- Add routes for:
  - `/about` -> responds with "About Page".
  - `/contact` -> responds with "Contact Page".
  - `/services` -> responds with "Our Services".
- Test each route in the browser.

# Exercise 3: Route Parameters
## Objective: Create dynamic routes using route parameters.
## Steps:
- Add a route `/user/:username` that responds with `Hello, <username>!`.
- Test the route by visiting paths like `/user/john` or `/user/jane`.

# Exercise 4: Using Query Parameters
## Objective: Handle query parameters in routes.
## Steps:
- Add a route `/search` that accepts a query parameter `q`.
- Respond with `Search results for: <q>`.
- Test the route by visiting paths like `/search?q=express`. The response should be `Search results for: express`

# Exercise 5: Using Express Router
## Objective: Organize routes using express.Router.
## Steps:
- Create a separate file (e.g., postRoutes.js) for post-related routes:
- `/posts` -> responds with "Posts".
- `/posts/:id` -> responds with "Post Details for ID: `id`".
- Import this router into the main app and use it with the path prefix `/api`.