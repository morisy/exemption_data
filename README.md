## Data Dictionary

* `exemption_id`: Currently, the full name of the jurisdiction plus a sequential ID made up of five digits, such as AK00001. Likely to be subject to future revision.
* `jurisdiction`: The jurisdiction that the exemption is applicable to. For exemptions that span multiple states, such as *McBurney v. Young*, each would have its own *McBurney v. Young* exemption with a different jurisdiction where it applies.
* `exemption_name` As canonical a name for the exemption as possible, for example, a specific legislative statute (), specific legal citation (i.e., "ACLU V. DEUKMAJIAN (1982) 32 CAL.3D 440, 452-453"), or term used for a specific category of rejection, such “Glomar Response” or “Constructive Denial.” 
* `status`: `Active`, if clearly still applicable and “live” law. `Repealed`, if repealed through statute. `Overturned`, if invalidated by court. `Active but Unsettled` if conflicting details on current status but still being regularly cited. `Unsettled` if highly ambiguous and not tested widely. 
* `type`: Legislative Exemption, Regulation, Advisory Opinion, Informal Exemption
* `alternative_citations`: Other ways that the exemption is referred to precisely. 
* `almost_certain_keywords`: Phrases that indicate a 90% or higher chance that the exemption is being invoked in a rejection letter.
* `likely_keywords`: Phrases that indicate a 60% or higher chance that the exemption is being invoked in a rejection letter.
* `related_exemptions`: The `exemption_id` of other exemptions that might have useful information for people researching a particular exemption, such as a parent exemption or a carveout.
* `examples_of_use`: MR numbers to requests that cite thie exeption OR URLs pointing off-MuckRock to examples of the exemption in the wild.
* `succesful_appeals`: MR numbers of requests where the exemption was succesfully appealed or links to detailed examples, including appeal language, where an appeal succesfully worked.
* `government_description`: A verbatim overview of the exemption provided by a government-source, pulled from the most comprehensive, authoratitve source available. Should be replaced if and when a superior source is created or discovered. Can range from language use in rejection letters to OIP/DOJ guidance.
* `government_description_source`: URL for the above.
* `exemption_description`: A requester friendly explanation of the exemption, including key information points about its proper application and strategies for overcoming.
* `contributors`: A list of comma-separated links including the names (or pseudonyms) of any contributors that wish to be identified as well as links back to homepages, MuckRock accounts, etc.
* `parent_exemptions`: If this exemption is a subset of another exemption or is the state implementation of a federal exemption, a link to the "parent" exemption.
* `case_law`: The names of any relevant litigation, formatted in markdown and, where possible, links to the most requester-friendly explanation of that case.
* `contributor_notes`: Internal notes such as flagging potential upcoming changes, areas for further research, etc.

## Common Exemption Categories

Many of these will directly correspond to specific statutes, case law, etc. within a given state. The most

 ### Requester Non-Responsive

The agency states that they have reached out and requested some sort of clarification or confirmation from the requester, but haven’t received any so they are administratively closing the request.

### Vague or Not Reasonably Described

The agency states that the request is asking for too much material, would require too extensive a search, or is otherwise not practical for them to process, and so they are rejecting or declining to process the request.

### Overly Broad or Unduly Burdensome

The agency states that the request is asking for too much material, would require too extensive a search, or is otherwise not practical for them to process, and so they are rejecting or declining to process the request.

### Materials Publicly Available

The agency states that the material requested is publicly available online and so they will not be directly providing the materials to the requester. They may indicate a specific place to look or generally indicate that the materials are available.

### Duplicate Request

The agency states that the requester has previously submitted a similar or identical request, and that it will not be also processing this new request.

### No Responsive Documents

The agency states that there are no responsive documents for the given request.

### Previously Completed

The agency states that it has already provided the records to the requester, but it is not providing the requested materials again in the current response. In some cases, the agency indicates that it will not provide the materials again in the future.

### Payment Required

The agency states that it has already provided the records to the requester, but it is not providing the requested materials again in the current response. In some cases, the agency indicates that it will not provide the materials again in the future.

### Agency Exempt From Law

The agency states that it has already provided the records to the requester, but it is not providing the requested materials again in the current response. In some cases, the agency indicates that it will not provide the materials again in the future.

