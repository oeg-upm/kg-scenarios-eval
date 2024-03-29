# WD-AMC

The WD-AMC dataset is a subset of Wikidata containing information about actors, movies and characters. It is provided in four representations (Standard Reification, N-Ary Relationships, RDF-star and Wikidata's Qualifiers) in RDF and KGTK format. Along with the datasets we include the queries used in the query performance scenario, that consists of 20 sets of 10 queries each created altering specific elements within each set, while the structure is maintained.

## Queries for the Query Evaluation Performance scenario

The following table represents one set of the queries in natural language.

| ID  | Questions  | Source   |
|-----|------------|----------|
| Q1  | Cast of the 2005 version of Pride and Prejudice | GoogleAI |
| Q2  | What character did Natalie Portman play in The Phantom Menace? | WebQSP |
| Q3  | Who won the academy award  for best actor in 2020? | GoogleAI |
| Q4  | Who is the Australian actress in blue Is The New Black?| GoogleAI |
| Q5  | How many movies have Woody Harrelson and Bill Murray been in together? | GoogleAI |
| Q6  | What movies did Sally Field win an Oscar for?| WebQSP |
| Q7  | What is the last movie Brittany Murphy made? | WebQSP |
| Q8  | Which actors were born on July 20th? | GoogleAI |
| Q9  | What was the cause of death of Sage Stallone?| GoogleAI |
| Q10 | Which characters and actors appear in both Breaking Bad and Better Call Saul? | GoogleAI |


## Queries for the Knowledge Exploration user study

A subset of these queries is used in the user study (Sets 1-4 of queries Q1-5) and can be seen in the following table.


| ID | Set 1                                                                                | Set 2                                                                       | Set 3                                                                       | Set 4                                                                   |
|----|--------------------------------------------------------------------------------------|-----------------------------------------------------------------------------|-----------------------------------------------------------------------------|-------------------------------------------------------------------------|
| Q1 | Cast of the 2005 version of Pride and prejudice                                      | Cast list of Alice in Wonderland by Tim Burton                              | Cast list of The Lord of the Rings: The Two Towers                          | Cast list of the movie Godfather 1972                                   |
| Q2 | What character did Natalie Portman play in star wars Episode I – The Phantom Menace? | What character does Ellen play in Finding Nemo?                             | What character does Mila Kunis play on Family Guy?                          | What character does Gary Oldman play in Darkest Hour?                   |
| Q3 | Who won the academy award for best actor in 2020?                                    | Who won the academy award for best actor in 2018?                           | Who won the academy award for best actress in 2015?                         | Who won the academy award for best actress in 2013?                     |
| Q4 | Who is the australian actress in Orange is the New Black?                            | Who is the spanish actress in Pirates of the Caribbean: On Stranger Tides?  | Who is the australian actor in Pirates of the Caribbean: On Stranger Tides? | Who is the israeli actress from Orange is the New Black?                |
| Q5 | How many movies has Woody Harrelson and Bill Murray been in together?                | How many movies have Johnny Depp and Helena Bonham Carter been in together? | How many movies have Emma Stone and Ryan Gosling been in together?          | How many movies have Tom Holland and Robert Downey Jr been in together? |



## Query performance evaluation results

The following table shows the results in seconds for the results of the evaluation of the Wikidata subset in Jena Fuseki 4.6.1. The lowest values of query execution time per query are highlighted in **bold**.

| Query      | Standard Reification | N-Ary Relationships | Qualifiers | RDF-star |
|------------|----------------------|---------------------|------------|----------|
|         **Q1** |                0.027 |               0.029 |      0.027 |    **0.017** |
|         **Q2** |                0.021 |               0.022 |      0.024 |    **0.019** |
|         **Q3** |                0.083 |               0.023 |      **0.022** |    0.522 |
|         **Q4** |                **0.020** |               0.028 |      0.023 |    **0.020** |
|         **Q5** |                0.081 |               0.034 |      0.024 |    **0.018** |
|         **Q6** |                0.065 |               0.022 |      0.021 |    **0.016** |
|         **Q7** |                0.018 |               0.022 |      0.022 |    **0.017** |
|         **Q8** |                0.441 |              62.566 |      0.433 |    **0.328** |
|         **Q9** |                0.019 |               0.023 |      0.019 |    **0.016** |
|        **Q10** |                0.031 |               **0.026** |      0.029 |    0.055 |
| **Total time** |                0.806 |              62.794 |      **0.641** |    1.029 |
