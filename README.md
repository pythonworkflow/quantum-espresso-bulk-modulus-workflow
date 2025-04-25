# Arithmetic Example Workflow
[![Pipeline](https://github.com/pythonworkflow/example-workflow/actions/workflows/pipeline.yml/badge.svg)](https://github.com/pythonworkflow/example-workflow/actions/workflows/pipeline.yml)

Template repository for publishing an interoperable workflow based on the Python Workflow Definition. 

## Content 
The minimal workflow consists of three files:

| File              | Explanation                                             |
|-------------------|---------------------------------------------------------|
| `environment.yml` | Conda environment for software dependencies             |
| `workflow.py`     | Python functions representing the nodes of the workflow |
| `workflow.json`   | Workflow graph consisting of nodes and edges            |

Additional optional files for the publication of the workflow: 

| File                             | Explanation                              |
|----------------------------------|------------------------------------------|
| `README.md`                      | Readme file to introduce the workflow    |
| `.github/workflows/pipeline.yml` | Github Actions to test the workflow      |

## Publish your workflow
You can publish your workflow in five simple steps:
* Fork the repository and clone your fork locally.
* Export your workflow to the Python Workflow Definition using the `python_workflow_definition` Python package, by calling the `write_workflow_json()` function.  
* Replace the `environment.yml`, `workflow.py` and `workflow.json` in your local folder with the files for your workflow. In addition, you can add additional files if they are required and update the `README.md` to explain your workflow.
* Commit the files locally using `git add -A` and `git commit -m "add my workflow"`
* Push your workflow to Github `git push`


