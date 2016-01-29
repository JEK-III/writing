
# Introduction
The California Digital Library (CDL) is seeking funding to incorporate RDA Working Group Recommendations into our data preservation and publication service, Dash.
Dash enables researchers from six University of California (UC) campuses to self-deposit data of any kind from any discipline to ensure preservation, enable citation via DOI, and enhance discoverability.
Individual UC campus libraries must opt-in to Dash and agree to pay data storage costs, at which point we set up a Dash instance for their researchers to use; consequently, both researchers and campus libraries are major stakeholders in the service.

Dash is run using enirely open-source software, primarily developed at the CDL.
Following an update planned for April, the Dash injest/discovery layer will interface with the underlying repository via standard protocols (SWORD, OAI-PMH), making the software broadly usable for general-purpose or discipline-specific preservation.
Although Dash is already a reliable and functional service, we have identified two key areas where RDA Working Group Recommendations could help us to offer a higher level of service: data metrics and repository certification.


# Data metrics
## Problem being addressed
Metrics of data impact/use are essential to incentivize data sharing by researchers.
The current Dash service does not collect or expose any metrics for the datasets or metadata records it contains.
The updated service will display a basic count of dataset downloads and metadata record page views.
While this is a good first step, the RDA-WDS Publishing Data Metrics Working group survey, as well as work carried out by the Making Data Count project, ntdemonstrated that researchers and data managers value citations above all else.
Consequently, we are seeking to collect and display a more complete set of metrics for Dash datasets.

## Nature of effort
For this project, we will integrate Dash with an in-development data metrics service hosted by DataCite.
We will modify Dash to collect metrics (i.e., downloads, views) in accordance with community standards being collected by the RDA Data Bibliometrics Working Group.
Then we will serve them via API to a lagotto instance being run by DataCite.
From DataCite, we'll get additional metrics, such as citations, collected for DataCite DOIs.
These will be displayed on landing pages and available for researchers, librarians, and administrators.

## Impact and metric of success
This project has the pontential to positively impact data sharing at a number of levels.
Researchers may be more likey to publish data if they can see that their data is being used; discovering citations to datasets is particularly likely to be motivating.
Campus libraries can better assess the value of the data being published through their library Dash portals.
This will help to justify funding for libraries to publish data.
For the world at large, increased adoption and display of data metrics will help to make the case that datasets should be valued as 'first-class' scholarly outputs.
<!-- how will we judge success of this particular program? -->

## Milestones
1. set up API to serve repository-side metrics to lagotto
2. begin collecting rich metrics from the lagotto API
3. design meaninful display for dataset landing pages


# Certification
## Problem being addressed
We believe that Dash/Merritt is a reliable preservation service, and we strive to adhere to best practices whenever possible, but we have never evaluated Dash relative to an external standard such as TRAC certification or the Data Seal of Approval.
Furthermore, although Dash is relatively recent, Merrit has been in operation for XX years, and standards may have evolved in the intervening years.
Rather than pick a standard at random, we would like to use the recommendations of the Repostiory Audit and Certification Working DSA-WDS Partnership WG to pursue certification.

## Nature of effort
Following the recommendation of the WG, we intend to use one of the existing 'entry points' to certification, the Data Seal of Approval.
Based on preliminary review of the certification criteria, our expectation is that current systems and policies are already near compliance. Most of the work will involve better documenting and formalizing current practices.
This work will involve :
1. reviewing the 16 DSA assement guidelines to identify what documentation must be collected, what de-facto practices and policies must be documented, whether any major changes must be made.
2. completing the online self-evaluation using the DSA tool and submitting for peer review.
3. making any changes recommended by the reviewers

## Impact / metric of success
The impact of this process will be to idenify and address any deficiencies in our current practices.
Formalizing and openly documenting our policies and practices will make the system easier for campus libraries and researchers to use.
Librarians and researchers will also be reassured that their data is safe with us.
A clear metric of success would be reciept of the DSA.
A secondary metric of impact might be an increase in dataset deposits following advertisement of the certification to the campus libraries.

## Milestones
1. complete review of existing practices relative to guidelines to determine the full scope of effort required
2. submit self-assessment
3. complete any changes required by peer review
4. recieve certification
