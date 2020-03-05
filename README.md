# Open-weather-api

Instructions to run the project:

1. Clone the aforementioned repository
2. Open postman navigate to below URL and post given payload using POST method.
  
http://localhost:8081/api/weather 

{
"name":"John",
"lastName":"Smith",
"dateTime":"31012019T1900Z", 
"country":"Australia",
"city":"Melbourne"
}

I have used global open weather API to get current temperature details. Final Output will be like below:

{
  "lastname": "Smith",
  "name": "John",
  "timeZone": "-18000",
  "fullName": "John Smith",
  "dateTime": "20200306170557013057",
  "temperatureCelcius": 294.33,
  "city": "Melbourne",
  "location": "Australia"
}

a. For full name I have append name & lastname.
b. timezone retrieved from global API.
c. date time is ISO format +1 day
d. temerature from global API

To get wetaher API details we need Apikey and country code which I mentioned in property files. Country Code I have hardcoded to AU.

For resuability, I have created global.xml file  where all configurations are defined.
