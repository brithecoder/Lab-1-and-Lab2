# Lab 1 Full-Stack Integration Analysis

## CORS Explained: In your own words, explain what a CORS error is and why it occurs in a typical MERN stack application with separate client and server repositories. Describe two different strategies a developer could use to resolve CORS issues during local development.

A cors or cross-origin resource sharing error is when a site or address doesnt have access to make calls or request to another program. Even though it is for protection it can sometime cause issues when your backend and front end are not properly set up to communicate. If you allow your backend to connect with the frontend by adding the frontend localhost port to your backend then they should be able to communicate.Sometimes people just add * for global access but this is not best for security you would probably want to add the frontend local host port and the the front end demain when it deployed. 

## Environment Management: Why is it considered a bad practice to hardcode API URLs directly into client-side React code? Explain how environment variables (.env files) help solve this on both the client (REACT_APP_...) and server (dotenv package).

Hmm I never heard it was a bad pactice to do that but I am guessing because maybe someone who knows how to access the codebase could find a way to make request to the API and if its not properly secured they could get access to sensitive data. It is possible that adding  the API in the .env and .env to .gitignore adds a layer of security. Using variables like REACT_APP_API_URL allows you to switch between a local address and a production address automatically depending on where the app is running.


## Data Fetching Trade-offs: The lessons covered both the native fetch API and the axios library for making API requests. Based on the resources and your own understanding, describe one key advantage of using axios over fetch for a complex application.

I think axioss is kind of like a way to make code cleaner and its sort of like a higer order function as it is doing what fetch does under the hood and axios automatically transforms the data into a javascript object as soon and the return comes back. 
