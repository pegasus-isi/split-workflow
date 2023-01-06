# Split Workflow 

# Dependencies
- Pegasus v5.0+
- HTCondor v10.2+
- Python 3.6+

![Split](https://user-images.githubusercontent.com/36110304/210929372-836122dc-d7cc-468f-80ce-7cf175f4e72a.png)

# File Description

<b>plan.sh:</b> Consists of all commands to be executed to run the workflow. Takes care of planning the pegasus workflow and initialising where the input files are and where output files should be located after execution of workflow. 

<b>workflow_generator.py:</b> Creates the abstract workflow, the replica catalog, the transformation catalog, and the site catalog. It has one job: split which is used to create the workflow. 

<b>Input Folder:</b> Contains all the input files to be used in the workflow.

# How to run the workflow?
```
# Plan and run the workflow generator to create an abstract workflow for the given input files
./plan.sh
`````
