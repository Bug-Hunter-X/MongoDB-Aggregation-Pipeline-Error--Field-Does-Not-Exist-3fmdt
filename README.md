# MongoDB Aggregation Pipeline Error: Field Does Not Exist

This repository demonstrates a common error in MongoDB aggregation pipelines: attempting to group or project on a field that might not exist in all documents after filtering.

The `bug.js` file shows the erroneous pipeline. The `bugSolution.js` file provides a corrected version that handles cases where the field is missing, using `$ifNull` to prevent errors.