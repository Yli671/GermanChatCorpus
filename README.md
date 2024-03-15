# GermanChatCorpus

This repository contains a corpus of elicited chat continuations in German.
The corpus combines informal (non-task-oriented) written dialogue with comprehensive annotations of both animate and inanimate referents, and coherence relations, essential for understanding natural communication.

## Data collection
To collect data, we simulated an interface similar to that of WhatsApp.
We created a set of chat dialogues (30 items) that included feedback utterances indicating grounding success or failure of a previous statement and asked our participants to write an appropriate continuation.
Data were collected from thirty native speaker of German, resulting in 900 chat continuations. Participants were recruited via Prolific.

## Data annotation 
The annotations were conducted with the web-based annotation software [INCEpTION](https://inception-project.github.io/). 
We annotated referring expressions (RE) and coreference relations between them, identified elementary discourse segments and their
types, as well as the coherence relations between these units.

## This repository
The structure of this repository is as follows:

- Folder **annotated_documents** contains the annotated documents in two format: (i) WebAnno TSV (Tab Separated Value) file format version 3, (ii) UIMA CAS XMI (XML 1.1). 
Each folder contains 30 documents corresponding to the 30 items in the experiment. And each document contains all the 30 chat continuations for that item. 
These files can be imported into WebAnno or INCEpTION for further annotations or into R/Python for analysis. 
The current version of the annotations (v1.0) contains golden coreference and segment annotations. However, the annotations of coherence relations are still ongoing and get continuously updated.