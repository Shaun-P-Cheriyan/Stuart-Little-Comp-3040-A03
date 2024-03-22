# API Documentation

The following is a pitch for the introduction of APIs into 3040Crypto's portfolio. Details will be provided, such as: a description of the API for context, a list of API endpoints, a description of resources in JSON format, and a sample request and output.

## API Description
We are proposing the inclusion of two APIs to add to our services. They are detailed below.
 - 3040Crypto's Crypto Tracker
   - Crypto Tracker will list a number of crypto currencies.
 - 3040Crypto's Crypto Value Tracker
   - Crypto value Tracker will display a specific coin's current exchange rate to USD.
   
   These are valuable to the company as they provide our users with the convenience of up-to-date information on crypto currencies.

## Endpoints 
3040Crypto's Crypto Tracker
 -  GET api/v1/coins/list
 -  Parameter : Num (Used to determine the number of cryptocurrencies to be displayed)
 -  Example Paramter Values : 0, 3, 5 (Here, input 0 corresponds to displaying all the crypto currencies) 

3040Crypto's Crypto Value Tracker
 - GET api/v1/coins/value
 - Parameter : Name (Used to determine the coin needed to be displayed)
 - Example Paramter Values : Bitcoin, Ethereum

## Resources 
3040Crypto's Crypto Tracker
~~~
{
    "Currencies" : [ ]
}
~~~
3040Crypto's Crypto Value Tracker
```
{
    "Id" : , 
    "Name" : ,
    "Value" : [ ] ,
    "Time" : 
}
```
## Sample
3040Crypto's Crypto Value Tracker

GET api/v1/coins/value?Name=Bitcoin
```
{ 
    "Id" : "1", 
    "Name" : "Bitcoin", 
    "Value" : ["USD", "60000"],  
    "Time" : "2024/03/18/182935" 
}
```
