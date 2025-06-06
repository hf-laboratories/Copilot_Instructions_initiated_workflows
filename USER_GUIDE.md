# User Guide

This guide will help end users understand how to use the application, including setup, features, and troubleshooting. (To be completed as the project evolves.)

add these instructions:

- When I type "workflows [workflow_name] [param]" in chat, recognize [workflow_name] as the workflow to run and [param] as its parameter.  
- Start a pwsh session.
- import copilot-workflows.ps1
- Execute the corresponding workflow function, with 'Handle-WorkflowCommand' passing the string 'workflows [workflow_name] [param]'
- For example, "workflows project document" should run the "project" workflow with "document" as the parameter, which generates project documentation.
- The return data will be a set of [instruction]s formatted like "Copilot Workflow: [workflow_fullname]", followed by a set of [instruction]s, one per line, which will describe each step required to complete a workflow followed by an 'End Workflow' string.
- For each workflow run, after receiving the output, submit a request to Copilot for each output line after the header line and up to (but not including) the 'End Workflow' line. Do not submit the 'End Workflow' line itself. All of these lines should be submitted as a single prompt.
- The format for workflow instructions is [instruction] [File_to_generate] eg. "Generate [File_to_generate]"
- the "generate" workflow is a call to action for you, copilot, to generate a file and populate it.
- If the instruction is 'Generate README.md, create a README.md file and populate it with contents describing the project.
- if the output instructions do not include a "End Workflow" line the intention is to complete the workflow up to that point and then press any key in the powershell to continue.
- the script will run skeleton population, then you should fill out the meat based on info from the project.
- After the workflow is run summarize work done and append the summary to a workflows-changes.md file.
  