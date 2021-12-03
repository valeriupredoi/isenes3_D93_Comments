## Comments needing extra info in text

### Comment 1
- Section 2.1, Paragraph 2
- Kim: "What happens to ESMValTool users that are not using these environments?"
- V inserted: "We are currently working on an extension of the observational data handler in ESMValTool, meant for users that don’t have access to th  ese HPC clusters, that will allow the local download of OBS data requested by the user."
- NOTE that this is detailed in Conclusions and Reccomendations below

### Comment 2
- Section 2.2, Paragraph 2
- Kim: "Is there a way to list the data downloaded by the user? This would be helpful to forward it to data managers to complete the ESGF da  taset."
- V answer off-document: no, there isn't since that would (probably) disagree with data privacy protocols; but we are working closer with CEDA on reporting these missing datasets, see https://github.com/ESMValGroup/ESMValCore/issues/1397
- V inserted: "We have started establishing a liaison mechanism between users requiring missing data (and eventually downloading it with ESM  ValTool) and HPC staff responsible for data replication, just so that we avoid such cases."
- NOTE that this is detailed in Conclusions and Reccomendations below

### Comment 3
- Section 2.2, Paragraph 2
- Kim RE "e.g. the tool is running on CEDA-JASMIN, for which the local DRS is BADC, but some data was downloaded from DKRZ’s ESGF node, so it comes packed in the DKRZ specific DRS, therefore the unified DRS to be used with downloaded data will be ESGF and must be set in the user configuration file:" says "Difficult to understand. I assume this needs human intervention to fix it."
- V rephrased to: "e.g. the tool is running on CEDA-JASMIN, for which the local DRS is set by the user in their configuration file to BADC, but some data was downloaded from DKRZ’s ESGF node, so it comes packed with a different directory structure than the data on CEDA-JASMIN (DKRZ, specific DKRZ DRS), therefore the the user should set the unified DRS to be ESGF, in their configuration file, to allow the use of both directory structures."

### Comment 4
- Section 2.3, Paragraph 3
- Kim: "Is the following text attached to Section 2.3? I don’t really understand why suddenly there are mentions to containers or installation methods."
- V answer off-document: we are talking about deployment (of ESMValTool) in central locations across HPC's, so container deployment is
  just another form of centrally-available deployment. Does this answer the query?

### Comment 5
- Section 2.4 - Title
- Kim:"I would mention the current manual intervention of the user to submit tasks in different machines and wait for the data. Perhaps it too ambitious and far away the scope of the project, but it would be nice to have a task manager that runs those jobs and produces the result."
- V: added at the bottom of Conclusions and Reccomendations: "Distributing tasks across HPC clusters will benefit from the implementation of a user-controlled task manager, that will assign tasks according to required memory intake, run time requirements etc.; such a task manager, akin the current cylc facility already in use at various sites, but extended to managing inter-HPC tasks, will be developed in close collaboration with the cluster maintainers."


### Rejected Comments

- "that reduce the input data volume[comma deleted] and run those on a machine that is close" - no, Cambridge comma needed :)

