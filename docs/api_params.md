# Overview
Our backend is able to accept a number of parameters via URL, i.e., task parameters and session identifiers.

## Session identifiers
activity_name: 

  - possible values: `symbol-search`, `grid-memory`, `color-shapes`, `color-dots`

admin_type: qualtrics, metricwire

study_id: a study identifier (name)

session_id: a session identifier

participant_id: a participant identifier

api_key: a valid API key ([reach out](mailto:m2c2@psu.edu) if you are ready to get started!)

group: a group indicator (str)

wave: a wave indicator (str)

## Task parameters

However although parameters are passed via URL, we still need to preserve type information to pass to m2c2kit. That happens by spelling the parameters **exactly** as noted in the links above, and the types need to be passed with a double color (::) seperator. For example, if I wanted 1 trial I would specify the URL param as: `number_of_trials=1::int`

See links below for all available parameters for each task: 

https://m2c2-project.github.io/m2c2kit/docs/schemas/grid-memory

https://m2c2-project.github.io/m2c2kit/docs/schemas/color-dots

https://m2c2-project.github.io/m2c2kit/docs/schemas/color-shapes

https://m2c2-project.github.io/m2c2kit/docs/schemas/symbol-search

## Example URL

The link below is an example of a task demo for Symbol Search, with 3 trials

https://prod.m2c2kit.com/m2c2kit/nt/index.html?activity_name=symbol-search&study_id=demo&api_key=demo&number_of_trials=3::int&show_quit_button=false::bool&participant_id=None&session_id=XXX&admin_type=missing