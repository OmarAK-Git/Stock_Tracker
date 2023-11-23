# Stock_Tracker
Insert desired stock name to monitor large positive or negative changes in stock price at end of day. If such events happen, sends an alert via text message to your phone with %Change - Description - Link to article. 
## Requirements and Instructions
<ol><li> Have a Twilio Account</li>
  Replace account_sid and auth_token within the code. 
<li> Sign up for free @ newsapi.org and alphavantage.co</li>
  Replace responding API tokens within the code. 
<li> Set the name and ticker of the stock you want to track  </li>
   constants named STOCK and COMPANY_NAME
<li> Select the size of % Change required to trigger the message  </li>
  Currently set to 5. 
</ol>

## Request Paths

<ul><li> GET https://www.alphavantage.co/query </li>
Params : Function, Symbol, Apikey
<li> GET https://newsapi.org/v2/top-headlines </li>
Params : Company Name, Catagory, Apikey, Language
</ul>
<br>
Note: As we are using the datetime moduel, beware when selecting when to run the code as your timezone might cause a delay in the trigger.  
