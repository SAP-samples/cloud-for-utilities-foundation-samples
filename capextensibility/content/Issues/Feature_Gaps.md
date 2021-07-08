1. **No extensibility for extending javascript files**.

   Currently no code extensibility - only modelled constraints

   new fields
   default values
   range check
   check against a value list (enum)
   new entity as code list
   new entity including an association pointing to it
   integrity check on an association
   new unique constraint (secondary index)
   mandatory check

2. **Sandbox for customer sandboxed extensions.**
   ->Investigation regarding WASM.
3. **Resetting extensions**.
   ->Currently this is on backlog for CAP.
   ->Only way is through an undocumented api.
   ->https://github.wdf.sap.corp/cdx/cds-mtx/blob/master/CHANGELOG.md#added-1
4. **UI**
   Although a UI does not need to be created by the provider, there is a lot of reliance in the auto code setup that makes it easier to use. Best would be for a consumer to create their own portal and link back to the main ui.However once again thisrequires a provider UI.Freestyle application seems the better way to go, however having problem accessing the extended service by itself.
5. **Tight coupling between the different concerns, UI/DB/Srv.**
   This can be overcome by using Cross-MTX but this is not their
   recommended approach.
6. **Activating must be done in extension folder**
   Currently if you create extension in the same directory as project
   and run cds activate it picks up the project directory and indicates
   extension activated.
