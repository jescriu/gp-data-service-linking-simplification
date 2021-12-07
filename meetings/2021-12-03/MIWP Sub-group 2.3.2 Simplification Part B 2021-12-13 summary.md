### MIWP Sub-group on Action 2.3.2 - Kick-of Meeting of Part B "Remapping of the extended capabilities" 

### Simplification of Data and Service Linking - Part B "Remapping of the extended capabilities" 

The meeting was held on-line (via WebEx) on 3rd December, 2021, 11:00 - 12:30 CET.

It was chaired by JRC and attended by experts from IT, NL, FR and DK.

#### Agenda:

1. Welcome and Approval of the agenda (JRC)
2. Possible amendments to [Part A Consolidated proposal (“Data-service linking simplification”)](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/blob/main/proposals/JRC/ds-linking-simplification-good-practice.md) (All)
3. Discussion on the Remapping of Extended Capabilities - [Based on Consolidated proposal – Annex B](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/blob/main/proposals/JRC/ds-linking-simplification-good-practice.md#annex-b) (All)
4. Way forward for Part B (All).
5. AoB (All).

#### Presentations:

[Presentation (PDF)](https://github.com/jescriu/gp-data-service-linking-simplification/blob/main/meetings/2021-12-03/20211203_MIWP_Sub-group_2.3.2_Simplification_Kick-off_Part_B.pdf)

#### Summary:

The JRC welcomed the attendees, provided an overview of the objectives of the meeting and proceed with the items scheduled in the agenda.

**Firstly, two items corresponding to [Part A Consolidated proposal (“Data-service linking simplification”)](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/blob/main/proposals/JRC/ds-linking-simplification-good-practice.md)** were discussed:
* Possible amendment of Part A Consolidated proposal proposed in [Issue #38](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/issues/38), to solve the lack of compliance of the Coupled resource implementation as per the Consolidated proposal:
As per the proposal in Issue #38 the URL of the Coupled resource should not be poining to the raw metadata, but to the #MD_DataIdentification section of the metadata.

Ine de Visser expressed her concerns about applying this pointer to the #MD_DataIdentification as a mandatory item - by the way, already included as TG Requirement 3.6 in the Technical Guidelines on Metadata v2.0.1 (TG MD) - because it is not widely used in current metadata despite it is required by the ISO standard. Hence, she proposed to allow more frienly metadata by just recommending the use of this pointer. The INSPIRE Reference Validator is not requiring it at the moment.

Antonio Rotundo added that it would be better to avoid repeating this requirement, which is already in the TG MD, and just make reference to it in the proposal for Part A.  

Fabio Vinci showed 3 different examples currently included in the TG MD to implement this pointer, but explained that it might not be useful in certain applications or clients if they do not process the #MD_DataIdentification pointer. Furthermore he clarified that if the applications / clients do process this pointer and as a result only the #MD_DataIdentification section of the metadata is retrieved. In this case, it could not be verified through the Resource Locator that the dataset metadata is the correct one - which is one of the objectives to be accomplished when applying Part A Consolidated proposal.

Since there was no agreement on a consensus solution to manage the issue, the group agreed to continue the discussion in the GitHub repository.

* Inputs sent by Heidi Vanparys on 2nd December:

**Secondly, **



#### Main points of the discussion (TBD) ####

XXX:
* xxx. 

#### Decisions:

1. .
2. 

#### Actions:

- [ ] The agreement on a consensus solution to manage [Issue #38](https://github.com/INSPIRE-MIF/gp-data-service-linking-simplification/issues/38) should continue in the dedicated GitHub repository.
