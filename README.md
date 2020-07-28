# Bwaise-sanitation-alternatives
This repository contains a model designed to evaluate the resource recovery potential, economics, and greenhouse gas emissions associated with three sanitation scenarios (the existing sanitation system and two alternatives) in Bwaise, Uganda.


The following files are contained in this repository, and all are necessary for the model to run:

Bwaise_sanitation_inputs.xlsx - This Excel spreadsheet allows the user to define the scenario being considered and edit all model parameter values and distributions used throughout the various modules.

Bwaise_sanitation_model.py - This Python script is the main code to be run when modeling a sanitation scenario. When this script runs, it imports the spreadsheet inputs and calls each function defined below to run through the entire sanitation system. Resources, costs, and emissions are tracked through each stage, and the results are output in a spreadsheet called Bwaise_sanitation_outputs

human_inputs.py - This function defines the excretion inputs entering the sanitation system

user_interface.py - This file contains a set of functions that call and run the user interface module specified in the input spreadsheet

decentralized_storage.py - This file contains a set of functions that call and run the specified decentralized storage module(s) specified in the input spreadsheet

conveyance.py - This file contains a set of functions that call and run the specified conveyance module specified in the input spreadsheet

treatment.py - This file contains a set of functions that call and run the specified treatment module(s) specified in the input spreadsheet

reuse_disposal.py - This file contains a set of functions that call and run the specified reuse/disposal module(s) specified in the input spreadsheet

lhs.py - This file assigns uncertainty distributions (via Latin Hypercube Sampling) to each parameter defined in the input spreadsheet
