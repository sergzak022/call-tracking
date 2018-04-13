# Call Tracking

## Description

This repository was created to assist in learning
call tracking functionality with voxology API. The tutorial
for it can be found [here](http://voxolo.gy/doc/call-tracking).

## Prerequisites

You'll need to provision at least 2 telephone numbers in order to follow along.

1. Create an account here https://portal.voxolo.gy, create an app and generate an API key.

2. Search for numbers with [`GET /PhoneNumbers/Available?{query_string}`](http://voxolo.gy/api-reference/#list-available-inbound-numbers).

3. Provision numbers with [`POST /PhoneNumbers/{inbound_api}`](http://voxolo.gy/api-reference/#provision-phone-numbers).

4. You should be able to see provisioned numbers at https://portal.voxolo.gy/v1/phone-numbers/inbound-numbers.

## Simple Call Forwarding

1. Modify `call-fllows/simple-call-forwarding.json` file (Don't forget to push changes to GitHub).

2. Assign this callback json file to the provisioned through Voxology phone numbers. Use [`PUT /CallFlows/Configurations/PhoneNumbers/{phone_number}`](http://voxolo.gy/api-reference/#update-call-flow-configuration).

3. Call the provisioned phone number.

## Time of Day Routing

1. Modify `call-fllows/time-of-day-routing.json` file (Don't forget to push changes to GitHub).

2. Assign this callback json file to the provisioned through Voxology phone numbers. Use [`PUT /CallFlows/Configurations/PhoneNumbers/{phone_number}`](http://voxolo.gy/api-reference/#update-call-flow-configuration).

3. Call the provisioned phone number.

## Advanced Call Forwarding

1. Modify `call-fllows/advanced-call-forwarding-leg-1.json` file.

2. Modify `cal1-fllows/advanced-call-forwarding-leg-2.json` file (Don't forget to push changes to GitHub).

3. Assign these callback json files to the provisioned through Voxology phone numbers. Use [`PUT /CallFlows/Configurations/PhoneNumbers/{phone_number}`](http://voxolo.gy/api-reference/#update-call-flow-configuration).

4. Call the provisioned phone number that registered with `call-fllows/advanced-call-forwarding-leg-1.json`.

## Shark Tank

1. Modify `call-fllows/shark-tank-customer-leg.json` file.

2. Modify `call-fllows/shark-tank-agents-leg.json` file (Don't forget to push changes to GitHub).

3. Assign these callback json files to the provisioned through Voxology phone numbers. Use [`PUT /CallFlows/Configurations/PhoneNumbers/{phone_number}`](http://voxolo.gy/api-reference/#update-call-flow-configuration).

4. Call the provisioned phone number that registered with `call-fllows/shark-tank-customer-leg.json`.

