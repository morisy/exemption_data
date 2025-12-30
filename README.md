One of the biggest challenges facing records requesters is what to do when agencies don’t actually provide the records, whether they reject the request with an arcane legal citation, tell a requester they’re request isn’t actually a proper request, or simply don’t respond. Our long-term goal with the exemption database is to build a database of every way that a request can go wrong — and tell users the best strategies for their next course of action.

Note that the exemption database includes entries for items that are not technically exemptions – maybe agencies in that jurisdiction tend to cite trade secrets, even though that's not an exemption written into law for that jurisdiction, for example, or else an agency rejects a request as a duplicate, even though that may not be prohibited. The database tries to be comprehensive regarding potential pitfalls, so it will include entries for those even though these withholdings are not necessarily based in law.

## Data Dictionary

* `exemption_id`: Currently, the full name of the jurisdiction plus a sequential ID made up of five digits, such as AK00001. Likely subject to future revision.
* `jurisdiction`: The jurisdiction that the exemption is applicable to. For exemptions that span multiple states, such as *McBurney v. Young*, each would have its own *McBurney v. Young* exemption with a different jurisdiction where it applies.
* `exemption_name` As canonical a name for the exemption as possible, for example, a specific legislative statute (), specific legal citation (i.e., "ACLU V. DEUKMAJIAN (1982) 32 CAL.3D 440, 452-453"), or term used for a specific category of rejection, such “Glomar Response” or “Constructive Denial.” 
* `status`: `Active`, if clearly still applicable and “live” law. `Repealed`, if repealed through statute. `Overturned`, if invalidated by court. `Active but Unsettled` if conflicting details on current status but still being regularly cited. `Unsettled` if highly ambiguous and not tested widely. 
* `type`: Legislative Exemption, Regulation, Advisory Opinion, Informal Exemption
* `alternative_citations`: Other ways that the exemption is referred to precisely. Separated by `|`.
* `almost_certain_keywords`: Phrases that indicate a 90% or higher chance that the exemption is being invoked in a rejection letter. Separated by `|`.
* `likely_keywords`: Phrases that indicate a 60% or higher chance that the exemption is being invoked in a rejection letter. Separated by `|`.
* `related_exemptions`: The `exemption_id` of other exemptions that might have useful information for people researching a particular exemption, such as a parent exemption or a carveout.
* `examples_of_use`: MR numbers to requests that cite thie exeption OR URLs pointing off-MuckRock to examples of the exemption in the wild. Separated by commas.
* `succesful_appeals`: MR numbers of requests where the exemption was succesfully appealed or links to detailed examples, including appeal language, where an appeal succesfully worked. Separated by commas.
* `government_description`: A verbatim overview of the exemption provided by a government-source, pulled from the most comprehensive, authoratitve source available. Should be replaced if and when a superior source is created or discovered. Can range from language use in rejection letters to OIP/DOJ guidance.
* `government_description_source`: URL for the above.
* `basis`: A requester-friendly explanation of the exemption, including key information points about its proper application. Where applicable, include the type of record the exemption blocks, such autopsies or commercial data. If there’s quotes from legal cases or government bodies’ opinions that describe this, go ahead and include that, including link backs to the citation in the most official place you can find it.  After reading this, people should have a general understanding of this particular way requests can be thwarted. Can be several paragraphs. *Accepts Markdown formating, including links.*
* `proper_application`: For this portion, describe examples of the “proper” or “right” way agencies should be using this exemption, if applicable. Sometimes, a request is properly rejected, and so this should provide context to let the requester know they need to try another route.
* `improper_application`: For this portion, describe examples of the “improper” or “incorrect” way agencies could be using this exemption. Maybe there’s an exemption to the exemption, such as predecisional information that’s over 25 years old.
* `example_appeal`: Ideally this is based off of a successfully filed appeal that we know has worked at least once, but even if you just try to put together a good guess at what the appeal would look like, it can be very helpful. Make sure to point to statute in the appeal, when necessary. You can include multiple appeals if there’s different paths that might be helpful. These should be written somewhat generically so that someone can copy and paste it and quickly adapt it to suit their specific situation. Seperate different appeals with `|`.
* `contributors`: A list of comma-separated links including the names (or pseudonyms) of any contributors that wish to be identified as well as links back to homepages, MuckRock accounts, etc. Over time, if someone overhauls an entry, we would include the original contributors names as well as the new contributors — we just keep adding and acknowledging folks.
* `parent_exemptions`: If this exemption is a subset of another exemption or is the state implementation of a federal exemption, a link to the "parent" exemption.
* `case_law`: The names of any relevant litigation, formatted in markdown and, where possible, links to the most requester-friendly explanation of that case.
* `contributor_notes`: Internal notes such as flagging potential upcoming changes, areas for further research, etc.

Formatting Notes: Some sections such as `examples_of_use` and `contributors` separate data points via commas. More complicated fields such as `example_appeal` separate data points via `|`. 

## Common Exemption Categories

Many of these will directly correspond to specific statutes, case law, etc. within a given state. In those cases, the specific statute should be cited, and these included in alternative citatinos. If no specific statute is known, just use these names as the name of the exemption.

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

### Ongoing Investigation

The agency states that the materials pertain to an ongoing or potentially ongoing investigation, and so are not subject to release.


