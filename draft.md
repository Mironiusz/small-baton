# AI and Machine Learning Inside HPC: A Scoping Review

## 2. Abstract

_To be completed._

## 3. Rationale

AI and ML are showing up more and more often in HPC research, but the field is scattered across different communities. That makes it hard for practitioners to quickly see what is actually being studied and which technologies seem promising, and what is still missing. A scoping review fits this goal well because we want to create a broad map of the area.

## 4. Objectives

This review answers three questions:

- **RQ1.** What problems in the HPC ecosystem need a machine learning solution?
- **RQ2.** What artificial intelligence and machine learning methods are used to solve these problems?
- **RQ3.** Which machine learning methods are used most often?

## 5. Protocol and registration

Before running the review, we prepared an internal protocol that defined the scope, research questions, search sources, inclusion and exclusion rules, and the data extraction fields. The protocol works as a lightweight operating manual for the review: it keeps the search, screening, and charting process consistent, even when papers use different terminology or come from different research communities. The protocol was not formally registered in an external repository.

## 6. Eligibility criteria

We will include papers where AI or ML is used to solve a problem inside HPC, such as autotuning, workload prediction, anomaly detection, scheduling, or performance modeling. We will exclude papers where HPC is only used to train AI models, papers about general AI for science without an HPC systems problem, papers without a real AI/ML method, and publications such as tool descriptions, keynotes, editorials, or short posters without a clear method. We will also exclude papers published before 2020 and papers not written in English.

## 7. Information sources

The core database search will be run in Scopus, Web of Science Core Collection, IEEE Xplore, and ACM Digital Library. We will also use manual search to identify important papers and to build a representative test set for checking whether the search strategy captures relevant work. The date of each search will be recorded and reported in the final review.

## 8. Search

We will perform both database search and manual search.

The search will use three term groups: AI/ML, HPC, and system-level HPC problems. The main query will be tested on a small set of known relevant papers and then adapted to each database syntax. Searches will target title, abstract, and keywords where supported. The search will be limited to English-language papers published from 2020 onward.

Planned base query:

```text
("artificial intelligence" OR "machine learning" OR "deep learning" OR "neural network*" OR "reinforcement learning" OR "graph neural network*" OR "predictive model*")
AND
("high performance computing" OR HPC OR supercomput* OR "parallel computing" OR "cluster computing" OR exascale OR petascale OR "heterogeneous computing")