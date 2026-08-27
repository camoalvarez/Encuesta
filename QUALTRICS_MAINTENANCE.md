# Qualtrics maintenance notes

This repository is an operational dependency of a Qualtrics survey. Survey stimuli are served from files in the `main` branch.

## Do not break existing survey references

While the survey is active or may be reused:

- Do not rename existing stimulus files.
- Do not move existing stimulus files to another directory.
- Do not delete stimulus files that may still be referenced by Qualtrics.
- Do not change the repository name or default branch without updating and testing all Qualtrics references.
- Prefer adding a new file with a new filename rather than replacing an existing stimulus when the visual content changes materially.

## Safe update procedure

When a stimulus must be changed:

1. Identify every Qualtrics question or embedded-data rule that references the file.
2. Add the new stimulus under a new, stable filename when possible.
3. Update the corresponding Qualtrics reference.
4. Preview and test the survey end to end.
5. Only remove an old stimulus after confirming it is no longer referenced anywhere in the active or reusable survey.

## Repository role

This repository hosts survey-facing assets only. The canonical experimental-design code, research data, empirical analysis, and publication documentation belong in the separate research repository.

## End of survey lifecycle

Once the survey is permanently closed and no longer needs to be maintained or reused, this repository can be converted into a historical archive. Before archiving it, preserve a record of the final Qualtrics version and the exact stimulus files used in that version.
