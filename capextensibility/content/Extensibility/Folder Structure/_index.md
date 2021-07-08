## The Extension Project Folder Structure

Before starting our project it makes sense to understand the extension
folder we have extended:

As you have noticed the folder structure consists of the following
directories:

```
.
├── CAP Directory Structure
├── db
│ ├── This folder is where you put your extensions of entities and UIs (Fiori Elements). (link to fiori elements?)
│ └── (see db inside node\_modules for reference of models which can beextended)
├── node_modules
│ └── Expanding this folder you will notice an embedded structure:
├── This is the reference models and services exposed that you are able to extend.
│ └── base
│ └── _i18n : This contain the i18n of the provider.
│ ├── Open the file and see the i18n keys and values.
│ ├── db : The entities available to extend./
│ │ ├── (The following is an example of the exposed list)
│ │ ├── Please refer to released documentation to understand in detail the referenced
│ │ └── entities.(get link)
│ │ └── models
│ │ ├── alpha
│ │ │ ├── configuration
│ │ │ ├── external
│ │ │ ├── mdiclient
│ │ │ └── serviceprovider
│ │ ├── extensions
│ │ │ ├── dpp
│ │ │ ├── BusinessPartnerServiceProviderExtensions.cds
│ │ │ ├── CustomerOrderUtilitiesExtensions.cds
│ │ │ └── Index.cds
│ │ └── odm
│ │ ├── billingaccount
│ │ ├── businesspartner
│ │ ├── common
│ │ ├── finance
│ │ ├── orgunit
│ │ ├── procurement
│ │ ├── product
│ │ ├── sales
│ │ └── index.cds
│ └── srv: The services that can be extended. (The following is an example of the exposed list)
│ ├── alpha
│ ├── api
│ ├── dpp
│ ├── external
│ ├── monitoring
│ ├── cds-mtx-auth.cds
│ └── service.cds
├── srv
└── This folder is where you put your extensions of services. (see srv inside of node_modules for reference)
```

**Note**: There is also a node_modules directory inside of \_base,
this can be ignored.

Avoid running npm install otherwise it will delete the \_base folder.