# M2C2kit Overview

[`m2c2kit`](https://m2c2-project.github.io/m2c2kit/) is a Typescript/Javascript framework for rapid-creation and iteration of cognitive assessments.

For more information about creating your own m2c2kit tasks, visit our documentation:

https://m2c2-project.github.io/m2c2kit/ 

## Overview: Using URL-based approach in your study

The link below is an example of a task demo for the Symbol Search cognitive assessment, with 3 trials

https://prod.m2c2kit.com/m2c2kit/nt/index.html?activity_name=symbol-search&study_id=demo&api_key=demo&number_of_trials=3::int&participant_id=XXX&session_id=XXX&admin_type=metricwire

The rest of this guide (as well as pages linked below) covers additional parameters you may leverage to customize the experience in your study.

## Getting Started Workflow

1. **Initial interest:** If interested in using the M2C2kit assessments with our secure data backend, please contact m2c2@psu.edu and nur375@psu.edu. We will send an Airtable form to collect information about your study, IRB and team.

2. **Onboarding:**  We will send the appropriate integration guide (e.g., Qualtrics, Metricwire) depending on your study needs. We will register your study data users and register your study ID on our portal. We will return an API key, Study ID and test URLs containing this information.

3. **Verification:** Once your study is configured via your chosen integration partner, we ask that you verify all links and resulting data before launching your study. With our API documentation, you will be able to develop a dashboard if relevant for your project (e.g., in Retool, Streamlit, Dash, etc.).

4. **Liftoff:** We will provide a set of Python and R scripts with common data querying use cases addressed. Once your study is complete, we will arrange sharing of all raw data files.

## About this Repository of Integration Guides

With the web-based implementation of M2C2kit assessments, it is possible for them to be embedded via Qualtrics, REDCAP, and Metricwire (as well as anything else with a WebView[cite]).

This repository contains implementation guides for using M2C2kit. 

The `templates` folder will contain examples of different ways in which you may configure m2c2kit cognitive assessments, e.g., in Qualtrics. 

## Table of Contents

- Parameterizing tasks via URL, available params: [`docs/api_params.md`](docs/api_params.md)
- Qualtrics Integration guide: [`docs/qualtrics.md`](docs/qualtrics.md)
- Metricwire Integration guide: [`docs/metricwire.md`](docs/metricwire.md)