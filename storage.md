Storage is used to persist the model. 
The model can be stored in a variety of formats - XML/XMI, Draw.io diagram, YAML, JSON, database records, graph, ...
It is also possible to store/load models in multiple formats in multiple storage systems. 

This page provides an overveiw for several storage types.

## File system

The model can be stored as a file or files. 
For example, job seekers (candidates) can store the model 
on their computers and build a very detailed model of their skills and work experience
over time.

## Git, including GitHub and GitLab

The next level after the file system is Git - it adds versioning/time dimension.
Git repositories can be used to builds workflows as explained in [Process As Code](https://medium.com/nasdanika/process-as-code-7b5d5ef3d166) 
story. 

This can be useful with AI agents - a human can review what was changed by an angent and approve it (human in the loop).
For example, an agent performs a job search and commits results to a branch. 
On GitHub/GitLab it creates a pull/merge request.

Git-based storage allows to implement a distributed model with parts of the model stored in multiple repositories and branches and cross-referencing each other.

## Database

There are many types of databases - relational, graph, ...
Database storagre requiest extra effort to implement load/store logic and also requies a database engine.
This approach might be usefult in server-side/cloud scenarios.