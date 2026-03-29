# TxtNet-Desktop-Server

## Host instructions
1. Register for an account at [Twilio](https://twilio.com/), purchase a toll-free number with SMS capability, and purchase credits. (This project will not work with Twilio free accounts)  
2. Create a Twilio application for the number.  
3. Sign up for an [ngrok](http://ngrok.com/) account and download the ngrok application  
4. Open the ngrok directory and run this command: `./ngrok tcp 5000`  
5. Visit the [active numbers](https://console.twilio.com/US1/develop/phone-numbers/manage/incoming) page and add the ngrok url to the "A Message Comes In" section after selecting "webhook". For example: "https://xyz.ngrok.io/receive_sms"  
6. Download the TxtNet Browser [server script](https://github.com/lukeaschenbrenner/TxtNet-Browser/blob/master/SMS_Server_Twilio.py) and install all the required modules using "pip install x"  
7. Add your Twilio API ID and Key into your environment variables, and run the script! `python SMS_Server_Twilio.py`  
8. In the TxtNet Browser app, press the three dots and press "Change Server Phone Number". Enter in the phone number you purchased from Twilio and press OK!  
