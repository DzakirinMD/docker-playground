# Deploy React App in Docker

## Requirements
This react app should be deployed in a Docker container
### Image

1. The base image should use alpine OS with node 16 pre-installed 
2. Set the working directory to /app inside the container
3. Copy app files to the docker image
4. Install the app dependencies
    ### `npm install`
5. Build the app
    ### `npm run build`
    Builds the app for production to the `build` folder.\
    It correctly bundles React in production mode and optimizes the build for the best performance.
6. Expose port 3000 which the app will be running. Note: This is to show the developers the running port as Documentation. 
7. Start the app
    ### `npx serve build`
    This command will start the production build in port 3000
8. Tag the image as `my-react-app-image`


### Container
1. The application should map & run in port 80.
    Therefore, should access the web with http://localhost
2. Name the container as `my-react-app`


