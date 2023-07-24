# Comparison of Knowledge Graph Representations for Consumer Scenarios - Resources

[![DOI](https://zenodo.org/badge/570553668.svg)](https://zenodo.org/badge/latestdoi/570553668)

## Description 

This repository provides supplemental material for the analysing the differential impact of different knowledge graph representations (Standard Reification, N-Ary Relationships, Wikidata qualifiers, and RDF-star) in common consumtion scenarios, i.e., knowledge exploration, systematic querying and graph completion. The resources comprise the data, queries and notebooks used for producing the datasets and performing the evaluations. 

## Structure
This repository is structured as follows:
* `WD-AMC`: Dataset created as a subset of Wikidata with information about Actors, Movies and Characters. 
  * `data`: points to the Zenodo repository where the datasets are stored: [https://doi.org/10.5281/zenodo.7443837](https://doi.org/10.5281/zenodo.7443837)
  * `queries`: SPARQL queries in the four representations to carry out the evaluations for the knowledge exploration and systematic querying scenarios. They are extracted from natural language queries from the [GoogleAI](https://ai.google.com/research/NaturalQuestions/dataset) and [WebQuestionSP](https://paperswithcode.com/dataset/webquestionssp) QA benchmarks.
  * `notebooks`: used to create the dataset.
* `REF-Benchmark`: Extended version of the [REF-Benchmark](https://github.com/dgraux/RDFStarObservatory/tree/master/testSuits/REF-Benchmark) adding to the current representations N-Ary Relationships and Qualifiers
  * `data`: points to the Zenodo repository where the datasets are stored: [https://doi.org/10.5281/zenodo.7443837](https://doi.org/10.5281/zenodo.7443837)
  * `queries`: SPARQL queries to carry out the evaluations for the systematic querying scenario. 

## Author
* Ana Iglesias (Ontology Engineering Group - UPM)
