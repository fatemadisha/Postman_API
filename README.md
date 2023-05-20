## How to run this project
- Clone this project
- Open with Postman / Command Shell
- Run Command:  
```console 
newman run Restful-booker.postman_collection.json -e BatchIT.postman_environment.json
```
- Run Command for Report: 
```console 
newman run Restful-booker.postman_collection.json -e BatchIT.postman_environment.json -r cli,htmlextra
```

## Technology used:
- Postman
- Newman

## Prerequisite:
- Jdk
- Node Js
- Newman
- Html Report Library

## Newman and Report Installation Process:
- Newman Install Command:
```console
npm install -g newman-reporter-htmlextra
```
- Newman Html Report Install Command:
```console
npm install -g newman-reporter-htmlextra
```

## API Documentation:
<a href="https://documenter.getpostman.com/view/26933640/2s93m1a4tK" target="_blank">Documentation Link</a>

## Test case list:
1. ### Get All Booking Id
	> Using For getting all the booking id.
    > Here used GET method to get all the data.
	 {
        "bookingid": 836
    }
	
2. ### Create Booking
	> Create Data Sets Using the Dynamic Random Variables.
    > Here used POST method to create a new.

3. ### Verify Crated Booking Details
    > Here used GET method for getting the created data.
	> In the test case you need to validate the following field values:
	1. > First Name
 	2. > Last Name
 	3. > totalprice
	4. > depositpaid
	5. > bookingdates
	6. > additionalneeds

4. ### Create Authurization Token
	> Using Form Data with those data
    > Here used POST method for create a new authorised token
	1. username : admin
	2. password: password123

5. ### Update Booking
    > Here used PUT method for updating the data.
	> In the test case you need to validate the following field values:
 	1. > Only Message

6. ### Verify Verify Updated Booking Details
    > Here used GET method for getting the updated data.
	> In the test case you need to validate the following field values:
	1. > First Name
 	2. > Last Name
 	3. > totalprice
	4. > depositpaid
	5. > bookingdates
	6. > additionalneeds

7. ### Partial Update Booking
     > Here used PATCH method for updating data partially.
     > Here we used patch method for updating some details.
     Example :
        {
         "firstname" : "Kaniz",
         "lastname" : "Fatema"
          }

8. ### Delete Specific Booking
    > Here used DEL method for deleting a data.
	> In the test case you need to validate the following field values:
	1. > Only Message


9. ## Newman Report Summary:

    ![](ReportImage/Newman(part1).jpg)




