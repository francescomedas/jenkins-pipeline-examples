# Handling errors generated in a build

_Note: Unstable is the expected result for this build_

Particularly when there is some sort of long running process for testing 
or other 'leak' that may occur from a build generating an failure it's useful
to catch and handle it.

This example demonstrates the following:

 * Long running docker container to execute tests in
 * Failed test in the container (exit code non-zero)
 * Catch the failure and report
 * Mark the build as UNSTABLE (FAILURE would also be a valid case)
 * Carry out cleanup of the docker container
 * Carry on to the next step

If the preference was to fail the build immediately rather than proceed to the next stage
then instead of setting currentBuild.result it would be better to throw(err) after the clean up.