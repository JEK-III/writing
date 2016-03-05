Not quite a year-and-a-half ago, the California Digital Library (CDL) [launched Dash](http://datapub.cdlib.org/2014/11/03/announcing-the-dash-tool-data-sharing-made-easy/), a self-service data preservation and publication service available to researchers on partnering campuses in the University of California (UC) system.
This [multi-campus service](https://dash.cdlib.org/) evolved from [DataShare](http://datashare.ucsf.edu), a collaboration between the CDL and the [UC San Francisco library](https://www.library.ucsf.edu/).
Almost immediately after Dash launched, the CDL got to work on the next version of Dash, thanks to funding from the [Alfred P. Sloan Foundation](http://www.sloan.org/).
The focus of this effort has been on transitioning to a more flexible underlying architecture, and improving the user interface/experience, but we are adding a number of new features along the way.
Dash version 2 will be released later this spring– here's what to expect.

## New features
Although the focus of the new version was on refining existing functionality, Dash users can look forward to useful new features:
* **Embargo support:** Researchers will soon be able to deposit data under a limited-time embargo. While the intention is that all data deposited in Dash will eventually become public, depositors will be able to defer publication of archived data to a future date (e.g., until the publication of a related paper). This, along with *metadata publication* will enable them to obtain a DOI for a dataset that they aren't ready to make public.
* **Metadata publication:** Researchers will be able to supply metadata for a dataset, be issued a DOI immediately, then return at a later date to deposit the data.
* **Geospatial search and browse:** Thanks to the efforts of the [UC Irvine Library](https://www.lib.uci.edu/), the [UC Irvine Dash instance](http://dash.lib.uci.edu) enables researchers to deposit data with associated geolocation (points or a bounding box). Geospatial metadata will now be available to all Dash instances. Depositors will be able to supply points, bounding boxes, or named places (drawn from the [MapZen](https://mapzen.com/) vocabulary) and consumers can limit searches geographically using a [GeoBlacklight](http://geoblacklight.org/) map interface.
* **ORCID integration:** Depositors will be able to link their datasets to their [ORCID](http://orcid.org/) IDs.
* **More metadata:** Depositors will be presented with field for miscellaneous notes needed to use the data– effectively a "README.txt" for the dataset.

## Better User Experience
After conducting usability testing with the existing dash deposit workflow and a couple of alternatives, we decided not to change it.
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
The dash service uses a subset of the DataCite metadata schema.
Metadata schema support is encapsulated into a Ruby Gem to enable easy substitution of alternative schemas.
Thus, DASH could be used for discipline-specific repositories.
