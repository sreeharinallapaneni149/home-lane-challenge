<h3>API LIVE DEPLOYED URL : https://home-lane-challenge.herokuapp.com/</h3>

<b>STEPS TO SET UP THIS PROJECT IN LOCAL :</b>

1. Clone the Repository https://github.com/sreeharinallapaneni149/home-lane-challenge.git
2. run `npm install`
3. Use post man to test APIs.

<br>

<b>API DOCUMENTATION</b>    <br>

First You'll need the token to Access APIs.
So,     <br>

<b>API - Generate Token</b>      <br>
    URL : https://home-lane-challenge.herokuapp.com/generate-token      <br>
    METHOD : GET
    
<strong>*Note : copy the Token after it's generated, You'll need it later.</strong>       <br>

<b>API - Budget Homes</b> <br>
    URL : https://home-lane-challenge.herokuapp.com/data-service/budgetHomes    <br>
    METHOD : POST<br>
    HEADERS : {Authorization: Bearer `token`}<br>
    BODY : {minPrice: `price`, maxPrice:`price`, pageNumber:`number`}   <br>
    
    Example Body :      
                        {
                            "minPrice":2000,
                            "maxPrice":500000,
                            "pageNumber":1
                         }

<br>
<b>API - Sqft Homes</b>    <br>
    URL : https://home-lane-challenge.herokuapp.com/data-service/sqftHomes  <br>
    METHOD : POST<br>
    HEADERS : {Authorization: Bearer `token`}       <br>
    BODY : {minSqft: `sqft_living`, pageNumber:`number`}        <br>
    
    Example Body :      
                        {
                            "minSqft":2000,
                            "pageNumber":1
                         }
     
<br>
<b>API - Age Homes</b>     <br>
    URL : https://home-lane-challenge.herokuapp.com/data-service/ageHomes   <br>
    METHOD : POST<br>
    HEADERS : {Authorization: Bearer `token`}<br>
    BODY : {year: `year`, pageNumber:`number`}<br>
    
    Example Body : 
                       {
                            "year":2020,
                            "pageNumber":1
                        }

<br>
<b>API - Standard Price Predictor</b>      <br>
    URL : https://home-lane-challenge.herokuapp.com/data-service/standardPrices     <br>
    METHOD : POST<br>
    HEADERS : {Authorization: Bearer `token`}   <br>
    BODY : { pageNumber: `number`}
        
    Example Body : 
                       {
                            "pageNumber":1
                        }
