Setting Up SkyScanner API Integration
Prerequisites
Before you dive into the code, make sure you’ve completed the following steps:

Sign Up on RapidAPI:
If you haven’t already, sign up on RapidAPI.
Search for the SkyScanner API and subscribe to it. This will give you an API key.
Remote Site Settings:
In your Salesforce org, navigate to Setup (the gear icon) > Security > Remote Site Settings.
Click New Remote Site.
Fill in the details:
Remote Site Name: SkyScanner_API
Remote Site URL: https://sky-scanner3.p.rapidapi.com
Check the box for Active.
Save your changes.
Adding the API Key
In your Apex class (SkyScannerApiCallout), replace 'YOUR_ACTUAL_RAPIDAPI_KEY' with your real RapidAPI key.

Java

public with sharing class SkyScannerApiCallout {
    private static final String BASE_URL = 'https://sky-scanner3.p.rapidapi.com/flights/search-one-way';
    private static final String RAPIDAPI_HOST = 'sky-scanner3.p.rapidapi.com';
    private static final String RAPIDAPI_KEY = 'YOUR_ACTUAL_RAPIDAPI_KEY'; // Replace with your real API key

    // Rest of your code...
}
AI-generated code. Review and use carefully. More info on FAQ.
Making the API Call
Now you’re all set! Your searchOneWayFlights method should work smoothly. Remember to handle the response data (likely in JSON format) appropriately.
