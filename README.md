LabVIEW Template Engine
=======================

The LabVIEW Template Engine is an example of how to use LabVIEW with the Dispatcher.


## How to start?

First you need an account at http://dispatcher.onlinelabs4all.org/ to create an Experiment Engine there. When creating an Experiment Engine you have to set a username and password for Basic authentication of the Web Services. The X-Apikey is generated automatically. Rename "config.dist.ini" to "config.ini" and update it with the information of the Dispatcher. Copy your VIs which control your remote lab into the "Lab_VIs" folder of the LabVIEW Template Engine. Open "Lab_Wrapper.vi" with LabVIEW, replace the "Lab_Dummy.vi" with the main VI of your remote lab and connect the inputs and outputs to the VI. Open "Template_Engine.vi" and update the constants in the state "PARSE ExpSpec" and "ASSEMBLE ExpResult", so that they match the schema of your Experiment Specification and Experiment Results.


## To Do

Currently the LabVIEW Template Engine can only parse the Experiment Specification and assemble the Experiment Results in XML. JSON is not yet implemented.


## Requirements

LabVIEW 2013 or higher
