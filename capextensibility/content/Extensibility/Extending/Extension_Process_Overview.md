The following documents a step-by-step process to extend C4U CO while
also providing in depth technical information that will allow you to
extend C4U CO functionality for your use cases.

**Please view the current **limitations** in the extension section of navigation.

C4U CO is built upon the [SAP Cloud Application Programming Model
framework](https://cap.cloud.sap/docs/) which allows C4U CO to focus on
exposing its vast domain expertise by:

- Focusing on the core domain and domain logic.
- Basing design on the models of the domain.
- Evolving the models by always collaborating with domain experts.

**CDS**

Since the primary focus of the framework is through [domain driven
design](https://martinfowler.com/bliki/DomainDrivenDesign.html) it makes
sense to familiarize yourself with SAP’s
[CDS](https://cap.cloud.sap/docs/cds/) universal modeling language. Once
you are familiar with CDS it will become easier to create both service
and database extensions.

CDS models are plain JSON objects that comply to the [Core Schema
Notation](https://cap.cloud.sap/docs/cds/csn) (An open specification
derived from JSON schema), which are in a very easily readable human
format. The models are what drive the CAP service runtimes and databases
as illustrated below:

<img src="../image1.png">

For complete documentation of CDS please refer to the following
[link](https://cap.cloud.sap/docs/cds/cdl#entity-and-type-definitions).



The following diagram shows the overall process that the extension developer will
follow to create an extension:

<img src="../Overview_Diagram.png">
