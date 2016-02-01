
# Introduction and project description
The California Digital Library (CDL) is seeking funding to incorporate RDA Working Group Recommendations into our data preservation and publication service, Dash.
Dash enables researchers affiliated with University of California (UC) campuses to self-deposit data of any kind from any discipline to ensure preservation, enable citation via DOI, and enhance discoverability and re-usability with rich metadata.
Individual UC campus libraries opt-in to Dash and agree to pay data storage costs, at which point the CDL establishes a campus Dash instance.
Consequently, both researchers and campus librarians are major stakeholders in the service.

Facilitating use of the Dash software platform beyond the UC system is a high priority in ongoing development.
Dash is run using open-source software, primarily developed at the CDL.
The service consists of an ingest and discovery layer, Stash (STore And SHare) and a preservation repository, Merritt.
Following an update planned for April, Stash will interface with Merritt via standard protocols (e.g., SWORD, OAI-PMH) to enable organizations to use Stash in conjunction with other underlying repositories.
Stash's modular architecture allows easy replacement of its default DataCite-based metadata with alternative schemas, making it broadly useful for general-purpose or discipline-specific data sharing.
Although Dash is already a reliable and functional service, we have identified two key areas where RDA Working Group Recommendations could help us to improve both the Stash platform and the Dash service: data metrics and repository certification.


# Data metrics
## Problem being addressed
The RDA/WDS Publishing Data Bibliometrics Working Group argues that metrics of dataset impact, use, and reuse are essential enabling technologies for recognition of researchers who publish valuable data.
A survey conducted by the working group found that metrics are also of high interest to administrators, data managers, and librarians who wish to evaluate the effectiveness of their services and target their efforts where they will be most effective.
The current Dash service does not collect, display, or expose via API any metrics for metadata records or datasets.
Th working group survey, and work carried out by the Making Data Count project ((http://mdc.lagotto.io/)[http://mdc.lagotto.io)) for Dash datasets as fully in accordance with working group recommendations as possible.

## Nature of effort
For this project, we will establish points of integration between the Stash dataset ingest/discovery layer and the open-source Lagotto metrics aggregation tool ((http://www.lagotto.io/)[http://www.lagotto.io/])– ideally in the form of an in-development data metrics service hosted by DataCite.
We will modify Stash/Merritt to calculate local metrics (e.g., downloads, views) in accordance with community standards (e.g., COUNTER, NISO outputs) being collected by the RDA Data Bibliometrics Working Group.
Stash will provide these metrics to Lagotto, which will compile additional metrics around social media activity and citations.
Drawing from Lagotto, Dash will display a meaningful set of impact metrics on dataset landing pages visible to researchers, librarians, and administrators.

## Impact and metric of success
Adoption of RDA/WDS Publishing Data Bibliometrics Working Group recommendations has the potential to positively impact data sharing within the UC system and beyond.
Researchers are more likely to publish data if they can see that their data is being used; discovering citations to datasets is particularly likely to be motivating.
Campus libraries can better assess the value of the data being published through their library Dash portals, which will help to justify funding for libraries to publish data.
Beyond the UC system, increased adoption and display of data metrics will help to make the case that datasets should be valued as 'first-class' scholarly outputs.

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


# Adopting organization

## California Digital Library
The CDL exists to support the University of California’s scholarship mission in an increasingly digital world. CDL’s diverse and talented staff has assembled one of the world’s largest digital research libraries, and has changed the ways that faculty, students, and researchers discover, access, use, and preserve information.
UC3 is a programmatic unit of the CDL and is a creative partnership bringing together the expertise and resources of the CDL, the ten UC campuses, and the broader international curation community.
Harnessing the collective energy and innovation of its partners, UC3 provides solutions that are out of reach of any individual partner.

## University of California
