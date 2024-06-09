# DJS08: React Router 


## Project Overview

[🎥 LOOM PRESENTATION LINK ](https://www.loom.com/share/13a9e4e819c4464083f98252105cd4aa?sid=73cd2e0c-b42c-431d-bb4b-ee926dffe07b)

For this challenge, we are required to code along with the lecturer from this lesson: [VanLife Project Bootstrapping](https://scrimba.com/learn/react/vanlife-project-bootstrapping-co8bc40b191eec875ecf00b23).

The starter code has all the CSS styling required for the project; you will just need to link the corresponding classes as you code along. Jump into the start code here: [GitHub Repository](https://github.com/CodeSpace-Academy/StudentNo_Classcode_Group_Name-Surname_DJS08/tree/main).

The focus for this project will be to understand routing and present our code.

## Discussion and Reflections

### Project Analysis 

**Project Setup and Configuration**
This project introduced us to React Router library and how to use them to make a single page application. Setting up and configuring the React Router is pretty easy, firstly all you have to do is run the command `npm install react-router-dom` and all the dependencies will be installed. Secondly you wrap the `App` component with `<BrowserRouter>` tag and define the `<routes>` and `<link>` inside.

**Route Params and nested Routes**
1. Route parameters are values that are passed as part of the URL path.
2.  The route `/vans/:id` defines a route parameter `id`. When a user navigates to `/vans/123`, the id parameter will be set to 123
3. The `useParams()` hook returns an object with the route parameters, and we can access the id parameter using destructuring.
4. We define nested routes by using the Route component inside another Route component
we have a top-level route for `/host`, and inside that route, we have several nested routes for `/host/income`, /host/reviews, /host/vans, and `/host/vans/:id`. The `/host/vans/:id `route has three nested routes for `/host/vans/:id`, `/host/vans/:id/pricing`, and `/host/vans/:id/photos`.

**Application of Route Parameters and Nested Routes + Implementation of Navigation Controls and Dynamic Linking**
1. The `<Link>` component from React Router enhances navigation within a React application by providing a way to declaratively navigate between routes
2. The `<Link>` component is used to create a "Back to all vans" button that navigates to the parent route (..) when clicked
3. NavLink is a variant of the `<Link> `component that provides additional features for styling active links. It's different from the basic `<Link>` component because it allows you to specify a style for the active link.
4. NavLink is used to create navigation links for "Details", "Pricing", and "Photos" sections. The style prop is used to specify an active style for each link, which is applied when the link is active.
5. Search parameters are a way to pass additional data in the URL query string
6. The useSearchParams hook returns an array with the current search parameters and a function to update them. You can use this hook to dynamically filter content based on the search parameters.


### Challenges and Reflections
This challenge was a mouth full because React Routers libraries has very complex and abstract logic. Some of the topics covered in the videos were a bit of a mind strech and I had watch them a couple of times to get an idea of what the concept really is and how to use it. Even now there are still concepts that I haven't fully understood fully and only through repeatative use will I be able to understand them. One concept the has eluded me is the `outlet` and `index` route.

## Author
Dimpho Molepo