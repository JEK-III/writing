# Dash DataPub Notes
two different posts here:
  * technical / feature-oriented
  * use-cases

## Technical Post
### Outline
* We announced Dash late in 2014
* What is Dash?
  * collaboration with the [UCSF library](https://www.library.ucsf.edu/)
  * researchers from participating can self-deposit data in our repository for preservation and publication.
* Dash v2 is coming this spring!
* funded by a Sloan Grant
* the three elements are
  * improvments in the UX
  * expanded features
  * under the hood

  * Better UX
    * similar, but streamlined workflow for deposit
    * prettier design
    * more readable metadata
    * modern, responsive design
    * tablet and mobile!

* New Features!
  * geospatial metadata and search for everyone!
    * MapZen placename lookup
  * embargoes!
    * deposit data to comply with data availability policies like [PLOS](http://journals.plos.org/plosone/s/data-availability) or [F1000 Research](http://f1000research.com/for-authors/data-guidelines)
  * metadata only!
  * ORCID integration: now, depostitors will be able to link to their ORCID IDs
  * more extensive metadata
    * notes field
  * PDF

* Under the hood
  * Loosely coupled via standard protocols
    * useable outside the CDL by pretty much anyone
  * modular design
    * easy to add metadata schemas
  * Ruby on Rails

* follow the project here?
* Credit UCSF

### Draft

Not quite a year-and-a-half ago, the California Digital Library (CDL) [launched Dash](http://datapub.cdlib.org/2014/11/03/announcing-the-dash-tool-data-sharing-made-easy/), a self-service data preservation and publication service available to researchers on parntering campuses in the Univerity of California (UC) system.
This [multi-campus service](https://dash.cdlib.org/) evolved from [DataShare](http://datashare.ucsf.edu), a collaboration between the CDL and the [UC San Francisco library](https://www.library.ucsf.edu/).
Almost immediately after Dash launched, the CDL got to work on the next version of Dash, thanks to funding from the [Alfred P. Sloan Foundation](http://www.sloan.org/).
The focus of this effort has been on transitioning to a more flexible underlying architecture, and improving the user interface/experience, but we are adding a number of new features along the way.
Dash version 2 will be released later this spring– here's what to expect.

## New features
Although the focus of the new version was on refining existing functionality, Dash users can look forward to useful new features:
* **Embargo support:** Researchers will soon be able to deposit data under a limited-time embargo. While the intention is that all data deposited in Dash will eventually becaome public, depositors will be able to defer publication of archived data to a future date (e.g., until the publication of a related paper). This, along with *metadata publication* will enable them to obtain a DOI for a dataset that they aren't ready to make public.
* **Metadata publication:** Researchers will be able to supply metadata for a dataset, be issued a DOI immediately, then return at a later date to deposit the data.
* **Geospatial search and browse:** Thanks to the efforts of the [UC Irvine Library](https://www.lib.uci.edu/), the [UC Irvine Dash instance](http://dash.lib.uci.edu) enables researchers to deposit data with associated geolocation (points or a bounding box). Geospatial metadata will now be available to all Dash instances. Depositors will be able to supply points, bounding boxes, or named places (drawn from the [MapZen](https://mapzen.com/) vocabulary) and consumers can limit searches geographically using a [GeoBlacklight](http://geoblacklight.org/) map interface.
* **ORCID integration:** Depositors will be able to link their datasets to their [ORCID](http://orcid.org/) IDs.
* **More metadata:** Depositors will be presented with field for miscellaneous notes needed to use the data– effectively a "README.txt" for the dataset.

## Better User Experience
After conducting usability testing with the exisitng dash deposit workflow and a couple of alternatives, we decided not to change it.
Users are led step-wise through the process of entering metadata, uploading files, checking for errors, and depositing their data.
However, the process has been streamlined in ways large and small.
e.g., DOIs will now be minted immediately on deposit, unlike the current system in which there is a delay.
Users can now move freely between steps in the process if they want.

The current fixed-width site will be replaced with a modern [responsive design](http://alistapart.com/article/responsive-web-design).
Desktop, tablet, and phone-optimized layouts will support reading, editing, and uploading.
The pages are being designed by [Randle Design](http://randledesign.com/) to lessen the frankly institutional feel of the current system, while also adhering more closely to UC branding guidelines.

## Flexible architecture
The current Dash is tightly coupled to the CDL's in-house repository, [Merritt](http://www.cdlib.org/services/uc3/merritt/)– making external adoption virtually impossible.
The next Dash will use standard protocols instead: [SWORD](http://swordapp.org/) for deposit, and [OAI-PMH](https://www.openarchives.org/pmh/) and [ResourceSync](http://www.openarchives.org/rs/) for metadata harvesting.
Consequently, it can sit atop any standards-compliant underlying repository.

Dash version two is a Ruby on Rails application.
The dash service uses a subset of the DataCite metadadata schema.
Metadata schema support is encapsulated into a Ruby Gem to enable easy subistitution of alternative schemas.
Thus, DASH could be used for discipline-specific repositories.









## Use-case driven post
### Outline
What can researchers do with Dash?
* deposit their data in a preservation repository
  * Dash service uses the CDL's Merritt repo; Campuses must pay storage costs, but that's it.
  * streamlined process
* publish their data to get credit
  * beautiful landing pages
  * citable: DOIs, citation strings
  * rich metadata
* satisfy publisher requirments
  * works fine for Nature Scientific Data, PLOS, F1000Research, etc.
  * can embargo data until publication of the associated paper
* satisfy funder requirments
  * works fine for most funders
  * can associate dataset with a specific funder and department drawn from FundRef
* publish data associated with a geospatial location
  * geospatial browse/search
  * location lookup using MapZen
* incorporate the dataset into their reference manager
  * download a PDF for reference
* read and download on the go
  * responsive design with mobile-optimized layour
  * takes adavantage of iOS and Android-mediated connections to cloud storage for download.


## Useful links

[Alfred P. Sloan Foundation](http://www.sloan.org/)
[ORCID](http://orcid.org/)
[announced Dash](http://datapub.cdlib.org/2014/11/03/announcing-the-dash-tool-data-sharing-made-easy/)
[OAI-PMH](https://www.openarchives.org/pmh/)
[SWORD](http://swordapp.org/)
[ResourceSync](http://www.openarchives.org/rs/)
[DataCite schema](http://schema.datacite.org/)
[MapZen](https://mapzen.com/)
[FundRef](http://search.crossref.org/fundref)
[UCSF library](https://www.library.ucsf.edu/)
[PLOS](http://journals.plos.org/plosone/s/data-availability)
[F1000 Research](http://f1000research.com/for-authors/data-guidelines)
[Merritt](http://www.cdlib.org/services/uc3/merritt/)
[Dash](http://dash.cdlib.org/)
[Randle Design](http://randledesign.com/)
[UC Irvine Dash instance](http://dash.lib.uci.edu)
[UC Irvine Library](https://www.lib.uci.edu/)
[GeoBlacklight](http://geoblacklight.org/)
[DataShare](http://datashare.ucsf.edu)
