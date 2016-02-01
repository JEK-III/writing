
# Introduction
The California Digital Library (CDL) is seeking funding to incorporate RDA Working Group Recommendations into our data preservation and publication service, Dash.
Dash enables researchers from six University of California (UC) campuses to self-deposit data of any kind from any discipline to ensure preservation, enable citation via DOI, and enhance discoverability.
Individual UC campus libraries must opt-in to Dash and agree to pay data storage costs, at which point we set up a Dash instance for their researchers to use; consequently, both researchers and campus libraries are major stakeholders in the service.

Dash is run using open-source software, primarily developed at the CDL.
The service consists of an ingest and discovery layer, Stash (STore And SHare) and a preservation repository, Merritt.
Following an update planned for April, Stash will interface with Merritt via standard protocols (e.g., SWORD, OAI-PMH) to facilitate adoption of the platform by groups using other underlying repository software.
In addition, Stash's modular architecture allows easy replacement of its default DataCite-based metadata with alternative schemas, making it broadly useful for general-purpose or discipline-specific data sharing.
Although Dash is already a reliable and functional service, we have identified two key areas where RDA Working Group Recommendations could help us to offer a higher level of service: data metrics and repository certification.


# Data metrics
## Problem being addressed
As demonstrated by the RDA/WDS Publishing Data Bibliometrics Working Group survey, metrics of dataset impact, use, and reuse are essential enabling technologies for recognition of researchers who publish valuable data.
Metrics are also valuable to administrators, data managers, and librarians who wish to evaluate the effectiveness of their services and target their efforts where they will be most effective.
The current Dash service does not collect, display, or expose via API any metrics for metadata records or datasets.
The next major release will display a basic count of dataset downloads and metadata record page views on individual landing pages.
While this is a good first step, the Publishing Data Metrics Working group survey, as well as work carried out by the Making Data Count project, demonstrated that researchers and data managers value citations above all else.
Consequently, we are seeking to collect and display a richer set of metrics for Dash datasets, in accordance with the working group recommendations to the fullest extent possible.

## Nature of effort
For this project, we will establish points of integration between the Dash dataset ingest/discovery layer and the Lagotto open-source metrics aggregation tool; ideally in the form of an in-development data metrics service hosted by DataCite.
We will modify Dash to ensure that the metrics (i.e., downloads, views) collected at the repository level are in accordance with community standards (e.g., COUNTER) being collected by the RDA Data Bibliometrics Working Group.
Repository-collected metrics will be served by Dash to the DataCite service.
From the DataCite service, Dash will receive additional metrics, such as citations and social media activity, collected for DataCite DOIs.
These will be displayed within Dash on landing pages and available for researchers, librarians, and administrators; they will also be available from lagotto.

## Impact and metric of success
This project has the potential to positively impact data sharing within the UC system and beyond.
Researchers may be more likely to publish data if they can see that their data is being used; discovering citations to datasets is particularly likely to be motivating.
Campus libraries can better assess the value of the data being published through their library Dash portals, which will help to justify funding for libraries to publish data.
For the world at large, increased adoption and display of data metrics will help to make the case that datasets should be valued as 'first-class' scholarly outputs.
Because Dash is open-source, Lagotto connections will be available for any other group that wishes to use the Dash ingest/discovery layer.

<!-- how will we judge success of this particular component? -->

## Milestones
1. set up API to serve repository-side metrics to lagotto
2. begin collecting rich metrics from the lagotto API
3. design meaningful display for dataset landing pages


# Certification
## Problem being addressed
In the development and operation of Dash, the CDL strives to adhere to best practices whenever possible, but Dash has never been evaluated relative to an external standard such as TRAC certification or the Data Seal of Approval.
It is possible that our procedures are inadequate and likely that additional documentation will be needed.
To ensure that Dash is fully complaint with recognized best practices, we intend to seek basic certification via the recommendations of the Repository Audit and Certification Working DSA-WDS Partnership Working Group.

## Nature of effort
Following the recommendation of the working group, we intend to use one of the existing entry points to certification, the Data Seal of Approval self-assesment tool.
Based on preliminary review of the certification criteria, our expectation is that current systems and policies are already near compliance.
Most of the effort will involve better documenting and formalizing current practices.
This work will involve :
1. reviewing the 16 DSA assessment guidelines to identify what documentation must be collected, what de-facto practices and policies must be documented, whether any major changes must be made.
2. completing the online self-evaluation using the DSA tool and submitting for peer review.
3. making any changes recommended by the reviewers

## Impact / metric of success
The major impact of this process will be to identify and address any deficiencies in our current practices.
Formalizing and openly documenting policies and practices will make Dash easier for UC campus libraries and researchers to use.
Librarians and researchers will also be reassured that their data is safe with us.
A clear metric of success would be successful certification.
A secondary metrics of impact might be increased data deposits following advertisement of the certification to the campus libraries or, ideally, adoption of Dash by additional UC campus libraries

## Milestones
1. complete review of existing practices relative to guidelines to determine the full scope of effort required
2. submit self-assessment
3. complete any changes required by peer review
4. receive certification
