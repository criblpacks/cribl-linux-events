# Linux Pack
----
the linux pack is designed to support the processing of linux OS data. it currently only support data being sent by a splunk universal forwarder. this pack includes sample logs for most of the inputs found in the Splunk TA for Nix, and includes three pipelines for processing said data. 

# Important Information
---
```
This pack may be incompatible with some Splunk dashboards that depend on specific field extractions.
Please review various Splunk add-ons and configuration files such as props.conf or transforms.conf and make adjustments as necessary.
```

# What to Expect
---
* Linux Filesystem Logs: Expect up to ??% reduction in the event size.
* [Splunk TA] linux scripted events:  Expect up to ??% reduction in the event size.
* [Splunk TA] linux scripted metrics:  Expect a range from ??% reduction in the event size.


# Installation
---
## Setup
To use this Pack, follow these steps:
1. Create a Route with with a filter for your Splunk TA Nix events and metrics and system logs, (see section below for recommendations on filters)
2. Select the `Linux` pack as the pipeline.

## Filter Suggestions
below are a few suggestions on filtering data to send to the Linux Pack.
- strict matching for linux scripted events: 
- strict matching for linux scripted metrics:
- match against host pattern: ```if all hosts with a specific name pattern run linux, this could be very effective```
- match against index: ```if you are routing all your linux data to a specific index, this could be very effective```
- match against file path: ```since linux paths use /, wild cards and log names should be enough```

## Updates
You can find most recent release at our repo [`releases page`](https://github.com/criblpacks/cribl-linux-events/releases) ~ link currently broken

## Release Notes

### Version 0.2 - 2021-11-30
almost completed pipeline for linux scripted event inputs from the 'Splunk TA for nix' and a generic pipeline for processing of metrics.

### Version 0.1 - 2021-10-31
partial pipeline for linux scripted event inputs from the 'Splunk TA for nix'.

# Odd & Ends
---
## Contributing to the Pack
To contribute to the Pack, please do the following:

email the author at the email address listed below

## Contact
To contact us please email acain@cribl.io

## License
This Pack uses the following license: [`Apache 2.0`](https://github.com/criblio/appscope/blob/master/LICENSE).
