# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.


# Login Profile, how useContext works?
In this application we need to pass the username 
So how it can be done?
Using useContext we can pass the data through the various components

# What is useContext?  how it works?
- The useContext hook in React allows components to consume values from the React context. React’s context API is primarily designed to pass data down the component tree without manually passing props at every level.
- It helps avoid the problem of "prop drilling," where props are passed down multiple levels from parent to child components.

# Working of useContext
- useContext hook consumes values from a React Context, making them accessible to functional components.
- First, create a Context object using React.createContext(), which holds the shared state.
- Use useContext to access the context value in any component that needs it, avoiding prop drilling.
- When the value of the Context updates, all components consuming that context automatically re-render with the new value.
- As per define in our application first we create one context folder and in that folder we create usercontext.js file in which we create one context object called userContext using react.createContext
- Now we create one userContextProvider.jsx file. The context which we created it provide a value that can be accessed by any child component wrapped in a Context.Provider.

# How it helpful for this application
- In this application we use useContext to pass the Username.