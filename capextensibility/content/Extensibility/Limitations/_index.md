The following are a list of known limitations in the CAP (Cloud Application Programming).

However this site may not contain the latest information - For the latest information please see the [latest community news](https://community.sap.com/topics/cloud-application-programming)

1. **No extensibility for extending javascript files**.

   Currently no code extensibility - only modelled constraints

   - new fields
   - default values
   - range check
   - check against a value list (enum)
   - new entity as code list
   - new entity including an association pointing to it
   - integrity check on an association
   - new unique constraint (secondary index)
   - mandatory check

2. **Extensions do not run in Isolation**

    Extensions are not run in isolation.


3. **Resetting extensions**.
   
    There is no way to remove all extensions and start over.


5. **Tight coupling between the different concerns, UI/DB/Srv.**

   It is possible to run separate the concerns however this must be done with Cross-MTA.
   Examples are provided [here](https://github.wdf.sap.corp/FE-SAMPLES/fe-samples-flp).

6. **Extensions can only be queried**

    Currently there is no tool exposing "what" was activated.


7. **PostgreSQL is not officially supported by SAP**

    There is some information [here](https://blogs.sap.com/2020/11/30/run-and-deploy-cap-with-postgresql-on-sap-cloud-platform-cloud-foundry-node.js/) should you wish to use CAP with postgres.
    

8. **No Version Control**

    Version controlling of the extension must be maintained by the implementor.


9. **Activating must be done in extension folder**

   Currently if you create extension in the same directory as project
   and run cds activate it picks up the project directory and indicates
   extension activated.
