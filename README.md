# Vault Ruby demo using Sinatra and MongoDB

This is a real basic example of the Braintree Vault in Sinatra using MongoDB to create a customer profile. Creates a customer and attaches a payment method, being stored in the Braintree Vault with the token being stored against the MongoDB profile. 

Once stored a token is returned that can be stored and transacted against as needed. 

The Mongo ID is stored in a custom field against the Braintree customer create as a future reference point, this will need to be setup inside the Braintree sandbox which can be done via Settings> Processing> scroll down to Custom Fields and create a field called 'profile_id'


## Technology

This demo uses

* Ruby 1.9.3 or higher
* MongoDB installed on the local machine with localhost:27017 available
* The [Sinatra](http://www.sinatrarb.com/) web framework

## Demo

* Fill in the following credentials:
  * Number: `4111 1111 1111 1111`
  * CVV: `123`
  * Expiration date: `11/2020`
* Click submit

or you can sign in using your PayPal Sandbox account

## Running the demo locally

* Run `bundle` to install all dependencies
* Run `ruby app.rb` to start the app
* Visit `http://localhost:4567/` in your browser
* Proceed as above
