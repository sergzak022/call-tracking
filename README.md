#Call Tracking

##Description

This repository was created to assist me in learning
call tracking functionality with voxology API. The tutorial
for it can be found here http://voxolo.gy/doc/call-tracking

##Prerequisites

You'll need to provision at least 2 telephone numbers in order to follow along.

1. Create an account here https://portal.voxolo.gy, create an app and generate an API key.

2. Search for numbers with `GET /PhoneNumbers/Available?{query_string}` (http://voxolo.gy/api-reference/#list-available-inbound-numbers).

3. Provision numbers with `POST /PhoneNumbers/{inbound_api}` (http://voxolo.gy/api-reference/#provision-phone-numbers).

4. You should be able to see provisioned numbers https://portal.voxolo.gy/v1/phone-numbers/inbound-numbers.

##Simple Call Forwarding

1. Modify `call-fllows/simple-call-forwarding.json` file.

2. Assign this callback json file to the provisioned through Voxology phone numbers.

3. Call the provisioned phone number.

4. If everything goes well you'll get redirected to the number that is specified in your call flow file.

##Time of Day Routing

1. 
