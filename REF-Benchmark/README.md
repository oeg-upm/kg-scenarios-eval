# REF benchmark

For the query performance scenario we used the [REF-benchmark](https://github.com/dgraux/RDFStarObservatory/tree/master/testSuits/REF-Benchmark) to compare different reification approaches. This benchmark provides the Biomedical Knowledge Repository (BKR) dataset in three representations: Standard Reification, Singleton Property and RDF-star. We extend this benchmark to evaluate two additional reification approaches: Qualifiers and N-Ary Relationships. For the Qualifiers, we apply the Wikidata model described in, introducing a statement resource that links the object as value and the added metadata as qualifier following the Wikidata URI schema. The N-Ary Relationships representation was built creating an intermediary resource that in turn links to the object and the added metadata.

## Evaluation results

The following table shows the results in seconds for the results of the evaluation of the REF benchmark in Jena Fuseki 4.6.1. The lowest values of query execution time per query are highlighted in **bold**.

| Query          | Standard Reification | N-Ary Relationships | Qualifiers| RDF-star |
|----------------|-----------|----------|-----------|-----------|
| **A-Q1**       |      **0.04** |    0.042 |     0.034 |     0.035 |
| **A-Q2**       |     0.664 |    0.364 |     1.342 |     **0.037** |
| **A-Q3**       |     0.923 |    1.478 |     **0.819** |   723.363 |
| **A-Q4**       |     1.476 |    1.765 |     **0.818** |   714.988 |
| **B-Q1**       |      0.03 |    0.033 |     **0.028** |     0.046 |
| **B-Q2**       |     0.499 |    0.285 |     **0.172** |    721.67 |
| **B-Q3**       |     0.776 |    0.413 |     **0.153** | 12909.028 |
| **F-Q1**       |     0.754 |    0.538 |     **0.376** |   730.174 |
| **F-Q2**       |    45.686 |   53.352 |    **36.230** |   752.959 |
| **F-Q3**       | 13737.903 | 10844.16 |  6284.461 |   **945.433** |
| **F-Q4**       |   669.387 |  385.483 |   161.378 |     **0.101** |
| **F-Q5**       |  2103.495 | 1235.367 |   505.814 |     **0.503** |
| **Total time** | 16561.633 | 12523.28 |  6991.625 | 17498.337 |
