#Sending SMS with curl

In this tutorial, you will use curl to send an SMS message to a mobile phone.

For [SMS API](https://www.sinch.com/sms-api/) pricing by destination, visit our [pricing pages](https://www.sinch.com/pricing/sms-prices/).

##Set Up
1. Create a Sinch developer account at [sinch.com/signup](#signup)
2. In the dashboard, click Apps in the left hand menu
3. Click create new app
4. Give your app a name and click create
5. Keep your app key and secret safe. You will need this in a minute
6. Open your terminal

##Sending the SMS via the API

Then, in the curl command, add the phone number and message you want to send, and add your app key and secret. Once you are finished, you should have something that looks like this:

````
curl --user "application\\your_app_key:your_app_secret" --data '{"message":"your_message"}' -H 'Content-Type: application/json' https://messagingapi.sinch.com/v1/sms/the_phone_number
````

Copy and paste this into your terminal, wait a few seconds and you should receive the SMS message to the phone number you added in the command.

##What's Next?

This is just a basic demo of our [SMS API](https://www.sinch.com/sms-api/) but read [our documentation](https://www.sinch.com/docs/rest-apis/user-guide/) and other [tutorials](https://www.sinch.com/tutorials/) to see how you can integrate this with your own backend. Any questions, just email the team at [hello@sinch.com](mailto:hello@sinch.com).
