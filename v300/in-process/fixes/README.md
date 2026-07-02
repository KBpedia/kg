# KBpedia v3.00 — Changes Log

This file records significant changes made during the v3.00 working cycle.
It serves as the basis for public release notes on version completion.

## URI Changes
- All hyphens in RC URIs replaced with underscores
- CamelCase splits applied where appropriate
- See changed_class_uris.csv and changed_prop_uris.csv for full listings

## Structural Changes
* Updated definitions
* Added relates_to property; applied to nearly 500 RCs (#76)
* Re-architected platform and revised overall directory structure
* Continued the trend toward greater reliance on Wikidata as an external resource
* Better organized living organisms under their respective taxonomic classifications
* Removed imbalanced, deep listings of specific species where they occurred
* Pruned intermediate RC assignments from typologies
* Generally pruned actual graph (#)
* Restructured large child branches (# 78)
* Tested and updated disjointedness assertions
* Reconciled the IDs for all RCs

## Assisting Program Changes
* Embraced and employed three different LLM coding assistants:  ChatGPT, Grok and Claude AI
* Created a local, filtered Wikidata dump to bypass SPARQL limits
* Codified support and statistical utilities for the knowledge graph

 ## Website Changes
  * Changed basis from Apache and Flask to nginx and Fast API
  * Removed need for Tomcat and Virtuoso
  * Added links and JSON metadata to individual instances from mapped external sources
  * Added thumbs to Wikidata-supported RCs

## Mapping Changes
* Remove wikipedia_categories.csv
* Removed dbpedia_categories.csv
* Added unspsc.csv
* Updated external mappings on Wikidata; got bot approval for updates
* <!-- Document Wikidata QID updates, new mappings, removed mappings here -->

## Notes
* All of this was undertaken while upgrading the AWS server and local desktop
* Employed an aggressive use of LLMs to assist in evaluation, analysis and coding tasks, specifically using ChatGPT (OpenAI), Claude (Anthropic) and Grok (xAI)
