# Clinic Management System



![clinic_manager](https://user-images.githubusercontent.com/52010932/208830805-63e96c8d-71e6-409a-8b92-0495e1726d96.png)


## Demo video
https://user-images.githubusercontent.com/52010932/209068272-5ee6b418-f7e2-4120-adf7-1b589165bdc3.mp4


## Introduction

A Clinic Management System is an integrated information system for managing all aspects of a medical clinic's operations such as medical, financial, administrative, legal, and compliance. It includes electronic health records, business intelligence, and revenue cycle management. 

The traditional clinic management system is a paper-based management system that has been used in the clinics for a long time. Based on this system, when a patient visits the clinic for the first time, the receptionist registers the patient and writes down his/her personal details in a form. The patient gets the treatment and takes the prescription with themselves given by the doctor. But this approach has been proven quite inefficient throughout the years which needs a quick update over the previous system. 



## Description

The Clinic Management system developed is basically a work assistance software that makes it easier to store the data of the doctors, receptionists and staffs who works in that clinic. It stores each of the patient data who visits the clinic. Their health record is also saved inside the database so that the doctor and receptionist can view that if needed. For new patients, the system generates a token value automatically after their registration and the receptionist will be in charge of awarding that token amount to the patients.

Overall, this system aims to make the whole process more efficient and flexible between the doctor, receptionist and patients.


## Visit the website
To visit the website, click here - [Visit website](https://front-desk-frontend.vercel.app/)

```
For login, use the following credentials - 

***Login as a Receptionist***
   username: suraj,
   password: hello
   
 ***Login as a Doctor***
   username: doctor123,
   password: hello 
```



## Available Scripts

In the project directory, you can run:

### `yarn start`


### `yarn test`

Launches the test runner in the interactive watch mode.
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject`

- ### Database design

  MongoDB is used to create the database of the overall system which is a NoSQL open-source document-based database. In MongoDB, data models are created according to the structure of the data which will be stored and it will be returned as a JSON object. 

  

- ### Designing REST API

  A REST API is designed which is used to perform the following tasks –

  - Get All data from the database (GET method).

  - Create data and store into database (POST method).

  - Update data (PATCH method).

  - Delete data (DELETE method).

  

   The github link of the REST API code:  (https://github.com/surajj2024/frontDeskClinic)
 
   The API is hosted on render web services. Visit here - [API link](https://frontdeskclinic.onrender.com/)
 



- ### Building Frontend

  ReactJS is used to design the frontend of the website which is an open-source front-end JavaScript Library for building UI interfaces. React Router is used to route different pages of the website. React Redux is used as a state container to read data from a redux store and dispatch actions to the store to update state i.e., it makes it easier to change the UI states in React. RTK query is a data fetching tool which is used to fetch data from the API linked above into the frontend.

  

- ### Authentication & Authorization

  - JSON Web Token is used to design the whole authentication system. JWT is a token based stateless authentication mechanism which is a client-side based stateless session where the server does not have to completely depend on the database to save session information.

    A JWT consists of three parts separated by period, they are as following ,

    ·    **HEADER:** It consists of token type and algorithm used for signing and encoding such as SHA256, RSA etc.

    ·    **PAYLOAD:** Payload consists of the session data called as claims such as Expiration time(exp), Issued at(iat) etc.

    ·    **SIGNATURE:** Signature is the most important part of the JWT. Signature is calculated by taking the header & payload and by encoding them 							using Base64url and concentrating them with a period separator. It is then given to the cryptographic algorithm. The signature 							changes when the header or payload changes and the private key is only in the hand of the Identity provider which prevents 							tampering the token.

    So, when a login happens, an access token along with a refresh token is sent. While the access token is available for short term, the refresh token life much more than the access token which helps you to login without typing your credentials for some days or weeks  

    

  - When the user hits an endpoint of the API, the received JWT token is sent to verify the protected resource by passing JWT in HTTP Authorization header & the resource server then authenticates the token using public key. The authorization used here is a role based authorization.



​															![jwt](https://user-images.githubusercontent.com/52010932/208853671-a71f1114-8194-4dd8-8698-8d5950174641.png)		


## Modules

The system consists of following modules – 

- **Receptionist login:** The receptionist is the user who can register itself in the software. After registration, they can log in to the system as the operator of the system. The receptionist have access to following features - 
  - View patients.
  - Add/delete/update a patient.
  - View doctors.
  - Add/delete/update a doctor.

 

- **Doctor login:** The doctor logs in to the system and examines all the patient’s details. Doctor can only view the patients record details.

 

- **Token generation:** The system will generate new token amount automatically for the new patients.

 

- **Patient information:** Along with prescription, patient information is recorded in the database.



## Technology stack

1. **React** , an open-source JavaScript frontend library used for designing the frontend.

   

2. **Redux**, an open-source JavaScript library used for managing application states.

   

3. **RTK Query **, a powerful data fetching and caching tool. It is designed to simplify common cases for loading data in a web application, **eliminating the need to hand-write data fetching & caching logic yourself**.

   

4. **Ant design & Material UI** , these are two open-source React UI library which have been used correspondingly for building elegant interfaces.

   

5. **Node.js**  , an open-source, cross-platform JavaScript runtime environment and library for running web applications outside the client's browser.

   

6. **Express.js**  , is a back end web application framework for building RESTful APIs with Node.js.

   

7.  **MongoDB**, a document-oriented database which uses JSON-like documents with optional schemas.

   

8.  **JWT**, an open standard used to share security information between two parties — a client and a server. it is used here for designing authentication system.

   



#   f r o n t D e s k F r o n t e n d 
 
 
