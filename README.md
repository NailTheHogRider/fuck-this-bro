# trainee-5-23t3

## Frontend

### Setting up the frontend
Open a terminal in the src folder at client/limit-frontend/src. Then install all npm packages with npm i. If starting from the outermost directory this will look like
```
cd client
cd limit-frontend
cd src
npm i
```
To run the frontend run the following command in the src folder
```
npm run dev
```

### Releveant documentation for the Frontend
* *React* (https://react.dev/)

* *Mantine* (https://mantine.dev/getting-started/)
    * We're going to use components from this library so that we don't need to build everything from scratch. Note for some of the backgrounds or more crazy styling effects you might need to create your own css styles, and just use them like you were using a html5,css,js website.
    
* *React Router* (https://reactrouter.com/en/main/start/tutorial)
    *  React doesn't have an inbuilt method of routing to multiple pages so we use this library
    * If you are having trouble with passing data between pages or html features (e.g. form submission) are behaving weirdly you might want to check this out

### Quick runthrough of how the frontend works
*Might be easier to follow if you have the relevant files open*

index.html serves as an entry point where React will make alerations to the html based on our code. In the html we load the script main.tsx in which the ReactDOM will be created and attached to the html.

Inside main.tsx we wrap all initialise the React component, Mantine Provider (Styler) and RouteProvider. The router object is responsible to rendering the correct components for each route. 

We've provided an example where pages can be rendered as parts of the appshell in the root page (with navbar etc.) or rendered seperately.

