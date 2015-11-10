#Sending SMS With cURL

In this tutorial, you will use cURL to send an SMS message to a mobile phone.

For [SMS API](https://www.sinch.com/products/sms-api/) pricing by destination, visit our [pricing pages](https://www.sinch.com/pricing/sms-prices/).

We've also made a video tutorial to guide you through the process.

<a href="https://www.youtube.com/watch?v=A36GmSKgnzU" target="_blank"><img src="/images/sending-sms-curl.jpg" 
alt="Send SMS in cURL" width="400" height="281" border="10" /></a>

##Setup
1. Create a [Sinch developer account](https://www.sinch.com/dashboard/#/signup)
2. In the dashboard, click “Apps” in the left-hand menu
3. Click “Create new app”
4. Give your app a name and click “Create”
5. Keep your app key and secret safe as you will need this in a minute
6. Open your terminal

##Sending the SMS via the API

Then, in the cURL command, add the phone number and message you want to send, and add your app key and secret. Once you are finished, you should have something that looks like this:

````
curl --user "application\\your_app_key:your_app_secret" --data '{"message":"your_message"}' -H 'Content-Type: application/json' https://messagingapi.sinch.com/v1/sms/the_phone_number
````

Copy and paste this into your terminal, wait a few seconds, and you should receive the SMS message to the phone number you added in the command.

##What's next?

This is just a basic demo of our [SMS API](https://www.sinch.com/products/sms-api/), but read [our documentation](https://www.sinch.com/docs/) and other [tutorials](https://www.sinch.com/tutorials/) to see how you can integrate this with your own backend. Have questions? Just email the team at [hello@sinch.com](mailto:hello@sinch.com).
