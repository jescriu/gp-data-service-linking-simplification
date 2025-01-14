### Fifth meeting of MIWP Sub-group on Action 2.3.2

### Simplification of Data and Service Linking 

The meeting was held on-line (via WebEx) on 11th November, 2021, 15:00 - 17:00 CET.

It was chaired by JRC and attended by experts from DE, IT, AT, NL, ES, FR, CZ, PL, DK and LT.

#### Agenda:

1. Consolidated proposal - Overview (JRC)
2.	Discussion on the proposal (all)
3.	Way forward for the action (all)
4.	AOB (all)

#### Presentations:

[Presentation (PDF)](https://github.com/jescriu/gp-data-service-linking-simplification/blob/main/meetings/2021-11-11/MIWP_Sub-group_2.3.2_Simplification_20211111_meeting.pdf)

#### Summary:

The JRC provided an overview of the consolidated proposal for Data-Service linking simplification based on the work performed by the sub-group till the date, and the previous outcomes (past meetings, comments and GitHub issues received).

The aim of this consolidated proposal is to arrive to a consensus-based approach for simplifying the linking between INSPIRE data and services while maintaining the relevant quality checks in the INSPIRE Geoportal for assuring an effective linkage of the reported INSPIRE resources.

Based on the current obligation to provide in the INSPIRE dataset metadata a resource locator for linking to each of the services providing online access to the datasets, the proposal explicitly states the obligation to provide at least two resource locators, one linking to a view service (e.g. WMS Capabilities document) and another linking to a download service (e.g. WFS Capabilities document). It also describes an interoperable approach for informing and encoding the parameters included in the resorce locator (protocol, application profile) reusing the codelists already available in the INSPIRE Registry.

As for the obligation to provide a link to the dataset metadata from the service offering / providing access to such dataset (coupled resource element), the consolidated proposal aims at linking the coupled resource through just using a simple URL pointing to the dataset metadata (without additionally informing the unique resource identifier of the dataset, which was previously used for performing further consistency checks), regardless of the scenario which is chosen for providing all required service metadata elements, namely:
* Scenario 1 - Service metadata element provided by linking to an external service metadata file: The URL pointing to the dataset metadata from the `operatesOn` element of the service metadata file.
* Scenario 2 - Service metadata elements provided within the capabilities of the service: The URL pointing to the dataset metadata either from the `wms:MetadataURL` or the `wfs:MetadataURL` standard elements of the capabilities document of the service, respectively depending on the nature of this service (WMS or WFS), or from an entry level `describedBy` link in the case of ATOM feeds/services.

The Pros and Cons of the consolidated proposal were also exposed to the members of the sub-group.

Several comments on the consolidated proposal were received before the meeting as [issues in the GitHub repository](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/issues). The final discussion with the audience was preceded by an explanation of the proposals / amendments for resolving these issues, which were prepared by the JRC in advance as [pull requests in the same repository](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/pulls):
* Issues [#20](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/issues/20), [#22](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/issues/22), [#23](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/issues/23), [#24](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/issues/24): Pull request [#31](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/pull/31).
* Issue [#21](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/issues/21): Pull request [#32](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/pull/32).
* Issue [#27](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/issues/27): Pull request [#34](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/pull/34).
* Issue [#28](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/issues/28): Pull requests [#35](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/pull/35) and [#36](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/pull/36).
* Issue [#29](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/issues/29): Pull request [#33](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/pull/33).

#### Main points of the discussion (TBD) ####

After the dicussion on the consolidated proposal, the sub-group was requested to provide input on the next steps to bring the work forward to an end:
* Endorsement of the consolidated proposal with the proposed amendments. 
* How to address the “Service simplification” topic (especially for removal of the Extended capabilities section from the service capabilities document).
* Assessment of the needs/opportunities to develop a specific conformance class in the INSPIRE Reference Validator to check the implementation of the simplified approach.

#### Decisions:

1. The agenda proposed for this meeting was approved without any modifications.
2. The [consolidated proposal for Data-Service linking simplificacion](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/blob/main/proposals/JRC/ds-linking-simplification-good-practice.md) was endorsed by consensus of all members of the sub-group attending the meeting, after the JRC presented the proposals (pull requests) for resolving the issues gathered in the GitHub repository within the period of consultation, which were also agreed by the sub-group.
3. With the aim of organising the continuation of the sub-group activities, the JRC proposed to close the first step of the simplification (Part A) and continue the activity of the sub-group for up to 6 months with a second step (Part B), as explained below:
  * **Part A. Data-service linking simplification**
This part of the work is considered to be **achieved** with the endorsement of the Data-Service linking simplification consolidated proposal, after merging the mentioned pull requests and performing a final quality check revision of the proposal by the JRC.
  * **Part B. Removal of the extended capabilities**
This part of the work will start just after this meeting, for a period of 4-6 months, with the objective to come up with a consolidated proposal for removing the extended capabilities section from the capabilities document of INSPIRE services without loosing content, and cover any other side-effects derived from it. 
Antonio Rotundo (IT), Ine de Visser (NL) and Marie Lambois (FR) volunteered to draft the proposal for removal of the capabilities, which will complete the simplification tasks of the sub-group by allowing OGC services to fulfil the INSPIRE requirements without offering any extended capabilities. The sub-group will, through a second step, be involved in the validation of the proposal.

#### Actions:

- [ ] The JRC will merge the pull request presented during the meeting for updating the consolidated proposal for Data-Service linking simplificacion based on the consensus of the sub-group.
- [ ] Marie Lambois (FR) will open a new issue in the GitHub repository to further analyse any possible inconsistencies between the consolidated proposal for Data-Service linking simplification and the ISO standards regarding metadata.
- [ ] The JRC will contact the INSPIRE Helpdesk Facilitators in order to possibly involved them in the final quality check revision of the consolidated proposal. This will include the analysis of any remaining issues which could be identified.
- [ ] The JRC will kick-off Part B of the simplification work (Remapping of the extended capabilities). The members of the sub-group which volunteered to participate in this  work will be approached in due time.
- [ ] The sub-group will validate, and possibly endorse, the proposal for removal of the extended capabilities.
