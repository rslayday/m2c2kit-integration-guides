# About this Repository

With the web-based implementation of M2C2kit assessments, it is possible for them to be embedded via Qualtrics, REDCAP, and Metricwire (as well as anything else with a WebView[cite]).

This documentation page contains an implementation guide for using Metricwire. 

## Getting Started - Using the M2C2kit Production Server

1. Login to Metricwire Catalyst | [https://catalyst.metricwire.com/](https://catalyst.metricwire.com/)

2. Create or edit an Assessment

![Assessment view](metricwire_assessment.png "Assessment view")

3. Add a Field of type 'WebView'

![Add `WebView`](metricwire_webview.png "Add `WebView`")

4. Enable `catalyst_next_button` event to go next

![Enable `catalyst_next_button` event to go next](metricwire_next.png "Enable `catalyst_next_button` event to go next")

5. Enter URL you received from our documentation or Project Coordinator. Make sure to modify URL to include magic params that inject identifiers from Metricwire:

`|*studyId*|` = Study Identifier
`|*userId*|` = Participant Identifier
`|*submissionSessionId*|` = Session Identifier

For example:
[https://api.m2c2kit.com/m2c2kit/nt/index.html?activity_name=symbol-search&study_id=demo&api_key=demo&number_of_trials=1::int&participant_id=None&session_id=05222d55-bc87-4c30-b756-c70ac9e62955&admin_type=metricwire](https://api.m2c2kit.com/m2c2kit/nt/index.html?activity_name=symbol-search&study_id=demo&api_key=demo&numb6er_of_trials=1::int&participant_id=None&session_id=05222d55-bc87-4c30-b756-c70ac9e62955&admin_type=metricwire)

6. Save changes, and sync the Assessment with your study.

7. Publish your survey and collect data!

### Data Access

Using this documentation would allow you to get started to collect data from m2c2kit assessments via Metricwire.

To get your data out of our backend, please contact [Dr. Nelson Roque](nur375@psu.edu) for coordination on using our API for data extraction.

## Getting Started - Using Custom Tasks

Guide coming soon!

## Metricwire Resources

Coming soon!