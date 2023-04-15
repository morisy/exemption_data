## Data Dictionary

* `exemption_id``: Currently, the full name of the jurisdiction plus a sequential ID made up of five digits, such as Alabama-00001. Highly likely to be subject to future revision.
* `exemption_name` As canonical a name for the exemption as possible, for example, a specific legislative statute, “Glomar Response,” or “Constructive Denial.” 
* `jurisdiction`: The jurisdiction that the exemption is applicable to. For exemptions that span multiple states, such as *McBurney v. Young*, each would have its own *McBurney v. Young* exemption with a different jurisdiction where it applies.
* `status`: Active, if clearly still applicable and “live” law. Repealed, if repealed through statute. Overturned, if invalidated by court. Active but Unsettled if conflicting details on current status but still being regularly cited. Unsettled if highly ambitious and not tested widely. 
* `type`: Legislative Exemption, Regulation, Advisory Opinion, Informal Exemption
* `synonyms`: Other ways that the exemption is referred to preicsely. 
* `signal_phrases`: Phrases that indicate a 80% or higher chance that the exemption is being invoked in a rejection letter.
* `potential_signal_phrases`: Phrases that indicate a 30% or higher chance that the exemption is being invoked ina rejection letter.
* `related_exemptions`: The `exemption_id` of other exemptions that might have useful information for people researching a particular exemption, such as a parent exemption or a carveout.
* `examples_of_use`: MR numbers to requests that cite thie exeption OR URLs pointing off-MuckRock to examples of the exemption in the wild.
* `succesful_appeals`: MR numbers of requests where the exemption was succesfully appealed or links to detailed examples, including appeal language, where an appeal succesfully worked.
* `government_description`: A verbatim overview of the exemption provided by a government-source, pulled from the most comprehensive, authoratitve source available. Should be replaced if and when a superior source is created or discovered. Can range from language use in rejection letters to OIP/DOJ guidance.
* `government_description_source`: URL for the above.
* `exemption_description`: A requester friendly explanation of the exemption, including key information points about its proper application and strategies for overcoming.
* `contributors`: A list of comma-separated links including the names (or pseudonyms) of any contributors that wish to be identified as well as links back to homepages, MuckRock accounts, etc.
* `parent_exemptions`: If this exemption is a subset of another exemption or is the state implementation of a federal exemption, a link to the "parent" exemption.
* `case_law`: The names of any relevant litigation, formatted in markdown and, where possible, links to the most requester-friendly explanation of that case.
* `tags`: TBD
