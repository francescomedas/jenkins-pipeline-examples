# Introduction

This repository is a home for snippets, tips and tricks and examples of scripting for the [Jenkins Pipeline plugin](https://github.com/jenkinsci/workflow-plugin/blob/master/README.md).

# Layout

The repository contains a sample Jenkinsfile each folder:

* *credential_handling* - for examples of how to get credentials from Jenkins vault.
* *error-control* - for examples of how to handle exceptions.
* *optional_steps* - for examples of how to implement conditional steps execution.
* *parametrised_scheduler* - for examples of how to implement a parametrised cron job.
* *require_manual_action* - for examples of how to define steps requiring manual intervention.

Please put your script into its own directory under the appropriate directory above, with a README.md file included explaining what your script does or shows. Make sure your script is commented so that others can understand how it works, why it works, etc.
