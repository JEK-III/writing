Best practice guidance
Multi-tenancy
Drag-and-drop upload
Metadata entry
DOI assignment
Embargoes
Faceted search and browse
Search engine optimization
Analytics
Dash is based on the Stash platform.  Stash is a Ruby on Rails application with three main components: Store, Harvest, and Share.
Pluggable protocol modules are encapsulated as Ruby engines for flexible deployment, (re)configuration, and extension.
It is loosely coupled to an underlying repository through standard protocols, such as **SWORD** and **OAI-PMH**.

Datasets are provided with scientifically-meaningful description using the DataCite metadata schema.  
Descriptive metadata is indexed for discovery using Blacklight.
Dash integrates with the wider research data management ecosystem through interoperation with Shibboleth and OAuth IdPs for
institutional single-sign-on, EZID and DataCite for DOI assignment and resolution, Scopus and Data Citation Index for high-level discovery, and ORCID
and Fundref for researcher and funder disambiguation

* External integrations
* * ORCID
* * FundRef
* * DataCite DOI

* Repository-agnostic
* * SWORD for deposit
* * OAI-PMH for harvesting

* Expandable
* * Plug-in architecture

* Out of the box support
* * DataCite metadata
* * Dublin Core

* Geospatial metadata
* *

Easy
* self-deposit via straightforward, familiar publishing workflow
* sign in with institutional credentials; no account to create or maintain
* automates data packaging and submission


Flexible
* works with any underlying repository using standard protocols
* pluggable architecture for additional protocols and metadata schemas
* deploy with single or multi-tenancy
