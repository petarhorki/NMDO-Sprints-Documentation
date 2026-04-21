Mappings
=========

Add mappings info


# Supporting work

## Orphacode driven disease group classification
For a batch import of records from an existing national rare disease registry into EURO-NMD, one interoperability challenge is how to classifiy a relatively large number of distinct Orphacodes (i.e. couple of thousands) to predefined EURO-NMD disease groups. To address this challenge, an Orphacode classifier (implemented scripts available on request) uses the Orphanet Rare Disease Ontology (ORDO) to automate this classification. Specifically, starting from predefined category roots, all ORPHAcodes that are subclasses/descendants of these roots are identified, and then assigned to the corresponding category.
The category roots are currently defined as follows:
*	Neuropathies: ORPHA:98496 — Rare peripheral neuropathy
*	Myopathies: ORPHA:98472 — Skeletal muscle disease
*	Mitochondrial Diseases:
    * ORPHA:225703 — Mitochondrial disease with peripheral neuropathy
    * ORPHA:68380 — Mitochondrial disease
*	Neuromuscular Junction Disorders: ORPHA:98491 — Neuromuscular junction disease
*	Motoneuron Diseases: ORPHA:98503 — Motor neuron disease

One limitation of this approach is that a single ORPHAcode may be assigned to multiple categories due to overlapping ontology hierarchies.
In addition to the above mentioned use, the list/mapping produced for classification by the implemented script can also support the effort of the NMD ontology.



