# BPIL Protocol 2018/2019
This repository contains a standard communications protocol for use during the Business Process Integration Lab course at the University of Twente. Intended consumers of the protocol (in the context of the case) are the various Transport Companies (TCs) and Distribution Centers (DCs).

## Protocol
This protocol lists the proposed methods supported by both Transport Company and Distribution center groups, including the expected input and generated output. Please refer to [protocoldc.jsonc](protocoldc.jsonc) and [protocoltc.jsonc](protocoltc.jsonc) for a descriptive implementation of this protocol. This protocol is subject to change, and discussion can take place in the [github issues](https://github.com/victorlap/BPIL-Protocol-TC-DC/issues).

All communication is done using XML-Schema (default for Mendix). Please refer to the [Mendix documentation of XML-Schema](https://docs.mendix.com/refguide/xml-schemas) based communication for more information.

## UUIDs
Throughout the service, UUIDs are used to identify objects. Other actors in the business process are encouraged to use this form of identification in their own web services as well. For more information on generating UUIDs in Mendix, please visit [this](https://forum.mendixcloud.com/link/questions/87680) page.