# Split Workflow 

# Dependencies
- Pegasus v5.0+
- Python 3.6+

![split-workflow](https://user-images.githubusercontent.com/36110304/212753610-843a44c9-9703-4dd1-9e50-86bd2a4deba7.png)

# File Description

<b>plan.sh:</b> Consists of all commands to be executed to run the workflow. Takes care of planning the pegasus workflow and initialising where the input files are and where output files should be located after execution of workflow.

<b>workflow_generator.py:</b> Creates the abstract workflow, the replica catalog, the transformation catalog, and the site catalog. It has one job: split This is used to invoke the executables which are present in bin folder.

<b>Input Folder:</b> Contains all the input files to be used in the workflow.

# How to run the workflow?
```
# Plan and run the workflow generator to create an abstract workflow for the given input files
./workflow_generator.py
./plan.sh workflow.yaml
`````
