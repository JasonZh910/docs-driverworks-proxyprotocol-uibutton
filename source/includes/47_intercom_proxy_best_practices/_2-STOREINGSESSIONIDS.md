## Storing Session IDs

Many intercom API commands and requests require the sessionId as an input parameter. The value for this parameter is provided by the SIP Client on the device in response to issuing a [`START_CALL`][1] command or a physical button press event. 

This sessionId value is included in the resulting [`OUTGOING_CALL`][2] or [`INCOMING_CALL`][3] notifications. The intercom proxy consumer is responsible for storing the sessionId returned with these notifications for use in subsequent commands and requests.

[1]:	https://snap-one.github.io/docs-driverworks-proxyprotocol/#intercom-call-commands-start-_call
[2]:	https://snap-one.github.io/docs-driverworks-proxyprotocol/#intercom-call-notifications-outgoing_call
[3]:	https://snap-one.github.io/docs-driverworks-proxyprotocol/#intercom-call-notifications-incoming_call