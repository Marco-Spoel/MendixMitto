# Mendix Mitto
Companies will use the Mitto module to communicate over SMS to their App users. The supported SMS types are next to the normal SMS, long SMS, Unicode SMS, bulk SMS (1 message to multiple numbers) and bulk SMS with callback. The callback function allows Mitto to update the application on the status of the SMS delivery per number in the bulk.  

## Mitto's Story
Since 2013, from locations all across the globe, we’ve been making communication happen. What began as a collaboration between a small team of telecommunications industry experts has grown into a powerful force of talent that is now ensuring best-in-class A2P messaging services for the largest brands in the world.
Our mission is to deliver reliable, high-quality communications between businesses and their customers, every time. Our team is given the support, tools, and freedom to make that happen.

## Typical usage scenario
Your company wants to send SMSes from the Smart App you are building. The Mitto service supports SMS, long-SMS, Unicode-SMS bulk SMS (1 SMS message to numbers) and SMS bulk message with a delivery report. The delivery report is received using a published REST API on /v1/callback.

## Features and limitations
The Mitto service uses security where you have to make available your breakout IP. This means that you need to give the Mendix Cloud IP ranges (see the documentation in the Module) and your company's Internet breakout for running the service on your development machine.
The callback API is not enforced by a security layer. As soon as Mitto Supports it, the next version will be published.

## Dependencies 
- Mendix modeller version 9.12.1 and higher
- Encryption
https://marketplace.mendix.com/link/component/1011
- Community Commons
https://marketplace.mendix.com/link/component/170
- Logging
https://marketplace.mendix.com/link/component/159
(for capturing logs on the free Mendix Cloud. Technically not required for sending the SMS)
- Excel Importer
https://marketplace.mendix.com/link/component/72

## Configuration 
See README in the Module
Known bugs 
- Regex validation error

# Frequently Asked Questions
-	Q: Why this module and not other SMS modules in the Marketplace?
-	A: Mitto has a rich service and a great price/performance
-	Q: Is Mitto a European company?
-	A: Yes, go to www.mitto.ch for all details
-	Q: Do I need the callback API
-	A: No, it is depending on the use cases. The callback report shows the status of the delivery of the SMS and provides you feedback on the quality of the numbers. If this help your data quality you can use it.

