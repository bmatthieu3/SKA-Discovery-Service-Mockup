# SKA-Discovery-Service-Mockup

This repository provides mockup responses to simulate the interaction with the Data Discovery Service. Both mockups are VOTables.

This is a 2-steps process:

1. the first step returns an [ObsCore](ObsCore) table. The *accessURL* field contains the link for the next step;
1. the [DataLink](DataLink) response contains two standard SODA services and an ad-hoc service resources field with metadata needed by the visualization tool (e.g., for VisIVO that is the backend location and dataset file path).

It is assumed that the client sends the proper HTTP User-Agent to get the customized DataLink output.

These files simulate Discovery Service responses for these queries. The responses return a datacube released in Apertif Data Release 1 and their location.

| **File** | **RA**     | **DEC**   | **Radius** | **Destination** |
|----------|------------|-----------|------------|-----------------|
| 001      | 215.02     | 56.83     | 0.2        | SPSRC           |
| 002      | 39.45      | 41.01     | 0.2        | ChinaSRC        |
