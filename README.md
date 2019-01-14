# BPIL Protocol 2018/2019
This repository contains a standard communications protocol for use during the Business Process Integration Lab course at the University of Twente. Intended consumers of the protocol (in the context of the case) are the various Transport Companies (TCs) and Distribution Centers (DCs).

## Protocol
This protocol lists the proposed methods supported by both Transport Company and Distribution center groups, including the expected input and generated output. Please refer to [protocoldc.jsonc](protocoldc.jsonc) and [protocoltc.jsonc](protocoltc.jsonc) for a descriptive implementation of this protocol. This protocol is subject to change, and discussion can take place in the [github issues](https://github.com/victorlap/BPIL-Protocol-TC-DC/issues).

All communication is done using XML-Schema (default for Mendix). Please refer to the [Mendix documentation of XML-Schema](https://docs.mendix.com/refguide/xml-schemas) based communication for more information.

## Tcid and Dcid
The Tcid and Dcid in the WSDL should be just your group number, to identify the different TC's and DC's

## UUIDs
Throughout the service, UUIDs are used to identify objects. Other actors in the business process are encouraged to use this form of identification in their own web services as well. For more information on generating UUIDs in Mendix, please visit [this](https://forum.mendixcloud.com/link/questions/87680) page.

## For TCs
Please assure you have updated to the latest version of the WSDL file from DCs (and click import):
https://raw.githubusercontent.com/victorlap/BPIL-Protocol-TC-DC/master/WebServiceDC.wsdl

![capture3](https://user-images.githubusercontent.com/1645632/51101810-8e59bb00-17dc-11e9-9351-f9efac584e2c.PNG)

And make sure your own exposed Web Services look like the following:

*RequestQuotations*
![whatsapp image 2019-01-11 at 15 00 09](https://user-images.githubusercontent.com/1645632/51101835-b5b08800-17dc-11e9-85b8-919efdd0b9ec.jpeg)

*AwardOrder*
`Image coming soon`

## For DCs
Please assure you have updated to the latest version of the WSDL file from TCs (and click import):
https://raw.githubusercontent.com/victorlap/BPIL-Protocol-TC-DC/master/WebServiceTC.wsdl

![capture4](https://user-images.githubusercontent.com/1645632/51101922-18a21f00-17dd-11e9-8cdd-160fa3d62fbb.PNG)

And make sure your own exposed Web Services look like the following:

*NotifyTruckArrival*

![capture5](https://user-images.githubusercontent.com/1645632/51101980-5acb6080-17dd-11e9-9a11-f352ec68c84f.PNG)

*GiveQuotation*

![capture6](https://user-images.githubusercontent.com/1645632/51101981-5acb6080-17dd-11e9-8f6d-4048ee8c28f4.PNG)
