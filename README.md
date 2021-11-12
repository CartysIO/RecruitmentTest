Review the figma designs here: https://www.figma.com/file/Dl1sA7tuIfP3vyeDzJqBgH/Persona-Clients-Screen?node-id=0%3A1

1. Create all UI elements in the Figma design:

2. Expected Behavior:
  a. All tabs should be functional, only one tab is designed, but the user should be able to move through tabs even if they are empty
  b. When a user clicks on a row entry (client) in the MY_CLIENTS_LIST view the app will open up the CLIENT_DETAILS_PAYMENTS for that client. 
  c. Inside the CLIENT_DETAILS_PAYMENTS there are two tabs - Payments and Sessions. Both should be functional, but only one will show data - payments
  d. All buttons will be designed even if not functional - you can print to logs the name of the button to show that it works
  e. The info presented 
  f. API calls and state management are to be made with Redux
  g. Android back button from CLIENT_DETAILS_PAYMENTS will lead to MY_CLIENTS_LIST

3. Server - in order to run the server first run `npm install` and then `json-server --watch db.json`. there are two endpoints: `/customers` and `/payments` for each one you query a single entry by id like so `/customer/1` or using query params for other types of filtering like so `/payments?userId=1234&status=open`. For more information about working with json-server read here: https://www.npmjs.com/package/json-server