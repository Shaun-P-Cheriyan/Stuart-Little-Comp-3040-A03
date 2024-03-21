# API Documentation

The following is a pitch for the introduction of APIs into 3040Crypto's portfolio. The following will be provided: a description of the API for context, a list of API endpoints, a description of resources in JSON format, and a sample request and output.

## API Description
We are proposing the inclusion of two APIs to add to our services. They are detailed below.
 - 3040Crypto's Crypto Tracker
   - Crypto Tracker will list a number of crypto currencies.
 - 3040Crypto's Crypto Value Tracker
   - Crypto value Tracker will display a specific coin's current exchange rate to USD.
   
   These are valuable to the company as they provide our users with the convenience of up-to-date information on crypto currencies.

## Endpoints 
3040Crypto's Crypto Tracker
 -  GET api/v1/coins/list/{all}

3040Crypto's Crypto Value Tracker
 - GET api/v1/coins/{coin-name}/value
## Resources 
3040Crypto's Crypto Tracker
> { <br>
>	    "Currencies" : [ ] <br>
> }

3040Crypto's Crypto Value Tracker
>{ <br>
>		  "Id" : , <br>
>		  "Name" : , <br>
>		  "Value" : [ ] , <br>
>    "Time" : <br>
>	}

## Sample
GET api/v1/coins/value?Name=Bitcoin
>{ <br>
>    "Id" : "1", <br>
>    "Name" : "Bitcoin", <br> 
>    "Value" : ["USD", "60000"], <br> 
>    "Time" : "2024/03/18/182935" <br>
>}
