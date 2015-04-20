# EUDAT Graph-based Data Integration

One of the challenges identified in the current CDI is to manage and represent relations between data objects. B2SHARE overcomes this limitation by providing its own metadata database, but this does not help for cases where information is put directly into B2SAFE or retrieved through other means such as the Generic Execution Framework.

To address this we propose to extend the persistence layer with a (distributed) graph database where such relations can be stored and retrieved. We will examine the applicability of this solution by implementing EUDAT-inspired use cases with the new technology. One possibility is the above-mentioned metadata use case. The challenge would be to store both data object and metadata record as "files" in the persistence layer and subsequently (like B2SAFE) make the relation between those two data objects explicit and visible in the graph. We will also seek a way of expressing the information that data objects stored on different sites through B2SAFE are actually the same, since replicated objects are clearly related to each other. This will lead to both an enriched service for EUDAT users who will be able to see the relationship between objects, and allow better resource handling since related data objects could be kept physically close (e.g., on the same tape if this is used at a site).

This task will work closely with WP5 and WP8 where work is planned looking at semantic web applications, data provenance and semantic annotation.
