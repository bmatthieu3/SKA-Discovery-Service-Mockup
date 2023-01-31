# SKA-Discovery-Service-Mockup

This repository provides mockup responses to simulate the interaction between VisIVO and the Data Discovery Service. Both mockups are VOTables.

This is a 2-steps process:

1. the first step returns an [ObsCore](ObsCore) table. The *accessURL* field contains the link for the next step;
1. the [DataLink](DataLink) response contains two standard SODA services and an ad-hoc service resources field with metadata needed by VisIVO.

It is assumed that the client sends the proper HTTP User-Agent (VisIVO/1.6) to get the customized DataLink output.
