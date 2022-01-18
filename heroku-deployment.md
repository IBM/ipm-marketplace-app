## Deploying the application on Heroku

#### Pre-requisites: 
- A public GitHub account

  Note: You can create an account using this [link](https://www.github.com/signup).
- Heroku account

  Note: You can create an account using this [link](https://www.heroku.com).
  
- Client Id and Client Secret

  Please follow this [doc]() to generate the required credentials.
  
#### Steps to deploy:
1.	Log into the GitHub Account.

2.	Navigate to the link: https://github.com/IBM/ipm-marketplace-app

3.	Fork the repository by clicking on the 'Fork' Button at the top right corner.

     <img width="640" height="400" alt="Screenshot 2021-11-10 at 8 48 07 PM" src="https://user-images.githubusercontent.com/41021851/141140453-6d023750-c8f4-4f81-8619-86a5c5d34624.png">

4. Navigate to this [link](https://id.heroku.com/login) and sign into the Heroku account.
 
   <img width="640" height="400" alt="Screenshot 2021-11-10 at 6 25 22 PM" src="https://user-images.githubusercontent.com/41021851/141141396-607dc3b0-5dfd-4a8f-8589-0eeecf75e4dd.png">

5. Click on 'Create new app' button in the dashboard.


   <img width="640" height="400" alt="Screenshot 2021-11-10 at 6 26 06 PM" src="https://user-images.githubusercontent.com/41021851/141142693-92a70a99-fb46-4c7f-a540-c5b8160372d2.png">

6. Provide a suitable app name, choose a region and click on the 'Create app' button.

    <img width="640" height="400" alt="Screenshot 2021-11-10 at 6 26 26 PM" src="https://user-images.githubusercontent.com/41021851/141146215-9f50ab7b-59c8-45a2-a4cb-a20a587b5b3c.png">

7. Click on the Github option under Deployment method.

    <img width="640" height="400" alt="Screenshot 2021-11-10 at 6 26 49 PM" src="https://user-images.githubusercontent.com/41021851/141154428-e540691d-425f-4fca-90fe-035966a586da.png">

8. Search and connect to the 'ipm-marketplace-app' repo.

    <img width="640" height="400" alt="Screenshot 2021-11-10 at 6 27 35 PM" src="https://user-images.githubusercontent.com/41021851/141155038-047a8d4d-6bb2-49fd-bc36-94e26403d34d.png">

9. Go to the Settings tab.
 
    <img width="640" height="400" alt="Screenshot 2021-11-10 at 6 28 14 PM" src="https://user-images.githubusercontent.com/41021851/141155859-e17004fa-77d0-4e61-836f-a65ba34e3e9e.png">

10. Under Config Vars, click on the 'Reveal Config Vars' button and add the following environment variables as key-value pairs.

    ```CCP_URL=https://wwwstage.ibm.com/marketplace/purchase/configuration```
    
    ```SA_URL=https://dev.api.ibm.com/marketplace/test/v2```
    
    ```CLIENT_ID=<generated-client-id>```
    
    ```CLIENT_SECRET=<generated-client-secret>```
    
       <img width="640" height="400" alt="Screenshot 2021-11-10 at 10 19 33 PM" src="https://user-images.githubusercontent.com/41021851/141157367-05347c79-8ebd-4ee0-9deb-6d28c7215872.png">

11. Go back to the Deploy tab and under Manual Deploy, click on the 'Deploy branch' button.

    <img width="640" height="400" alt="Screenshot 2021-11-10 at 6 28 04 PM" src="https://user-images.githubusercontent.com/41021851/141155422-ac8dc04f-da86-4ab0-932b-88acda65411d.png">

12. Check the 'View build log' option.

    <img width="640" height="400" alt="Screenshot 2021-11-10 at 10 27 48 PM" src="https://user-images.githubusercontent.com/41021851/141163448-c7b8903b-1a39-4181-8161-7be1b527a742.png">

13. Once the deployment is completed, click on the 'Open app' button.

    <img width="640" height="400" alt="Screenshot 2021-11-10 at 10 54 24 PM" src="https://user-images.githubusercontent.com/41021851/141163744-8de38310-e830-44cb-a564-7baaba54baa0.png">

14. Voila! The application is successfully deployed on Heroku :)

    <img width="640" height="400" alt="Screenshot 2021-11-10 at 10 54 33 PM" src="https://user-images.githubusercontent.com/41021851/141162859-58c05593-c79c-454d-b37c-a0f41216a010.png">
