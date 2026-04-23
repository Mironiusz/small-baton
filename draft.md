1. Title

AI and Machine Learning Applications in High-Performance Computing: A Scoping Review

2. Structured summary

This scoping review maps how artificial intelligence and machine learning are used to solve operational and optimization problems within high-performance computing systems. The review focuses on AI/ML applications in scheduling, resource allocation, workload prediction, performance prediction and modeling, anomaly detection, fault prediction, resilience, energy optimization, autotuning, runtime optimization, and HPC-oriented code optimization. The search strategy was built from AI/ML, HPC, and HPC problem terms and applied to Scopus, Web of Science Core Collection, IEEE Xplore, and ACM Digital Library. Retrieved records were merged, deduplicated, screened by title and abstract, and extended through snowballing. Included studies were classified by problem area, AI/ML technique, research type, evaluation type, HPC environment, and metrics. The review aims to identify the main application areas, dominant algorithmic families, evaluation practices, and research gaps in the field.

3. Rationale

Research on AI and ML in HPC is spread across multiple communities, including systems engineering, performance optimization, scheduling, and intelligent computing. As a result, the literature is heterogeneous in terminology, evaluation settings, and publication venues. A scoping review is therefore appropriate because the goal of this study is to map the existing body of research, identify the major areas of application, and highlight current research trends and gaps rather than to evaluate a single narrowly defined intervention.

4. Objectives

This review addresses the following research questions: (RQ1) What AI/ML application areas in HPC are described in the literature? (RQ2) Which artificial intelligence algorithms are used in these areas? (RQ3) Which algorithms are currently reported as the most effective? (RQ4) What HPC environments and evaluation metrics are used to assess these approaches?

5. Protocol and registration

A review protocol was prepared before the search and screening stages. The protocol defined the study scope, research questions, databases, preliminary search strings, eligibility criteria, screening procedure, data extraction form, and decision log. The review protocol was not formally registered.

6. Eligibility criteria

A publication was included if AI or ML was used to solve a problem within HPC, such as scheduling, resource allocation, workload prediction, performance prediction or modeling, anomaly detection, fault prediction, resilience, energy optimization, autotuning, runtime optimization, or HPC-oriented code optimization. A publication was excluded if HPC was used only as infrastructure for training an AI model, if the study addressed AI for science without an HPC systems problem, if it did not include a substantive AI/ML method, or if it was only a tool description, keynote, editorial, or short poster without a clear method. Studies published before 2020 were excluded.

7. Information sources

The main search was conducted in Scopus, Web of Science Core Collection, IEEE Xplore, and ACM Digital Library. Additional sources such as Compendex, Inspec, SpringerLink, or arXiv were considered optional extensions depending on availability and scope decisions. The review was further extended through backward snowballing, forward snowballing, and, if needed, manual inspection of selected publication venues.

8. Search

The search strategy was built from three concept blocks: AI/ML terms, HPC terms, and HPC problem terms. The AI/ML block included terms such as "artificial intelligence", "machine learning", "deep learning", "neural network*", "reinforcement learning", "graph neural network*", and "predictive model*". The HPC block included "high performance computing", HPC, supercomput*, "parallel computing", "cluster computing", exascale, petascale, and "heterogeneous computing". The problem block included schedul*, "resource allocation", "workload prediction", "performance prediction", "performance modeling", "anomaly detection", "fault prediction", resilience, "energy optimization", autotun*, "runtime optimization", "job placement", and "load balancing". Two queries were prepared: a broad query combining AI/ML and HPC terms, and a narrower query additionally restricted by HPC problem terms. The syntax of each query was adapted to the selected database, for example TITLE-ABS-KEY in Scopus and TS in Web of Science.

9. Selection of sources of evidence

The search process consisted of database querying, export of bibliographic records, merging of results into a single dataset, and deduplication. Records were then screened at the title and abstract level. Each record received one of three decisions: Include, Exclude, or Uncertain, where Uncertain was operationally treated as Exclude at this stage. A record was included if the title and abstract indicated that the study concerned HPC, used AI/ML, and applied AI/ML to an operational, system-level, or optimization-related HPC problem. The initial corpus was then extended through backward and forward snowballing with depth 1.

10. Data charting process

Data were charted using a structured extraction form prepared before the full analysis stage. The extraction sheet contained bibliographic, methodological, and classification fields and was designed to support both descriptive synthesis and cross-category comparison. LLM-based assistance was allowed only for article summarization and preliminary completion of selected extraction fields, and every such output required manual verification before inclusion in the final dataset.

11. Data items

The extraction form included the following fields: ID, source type, database origin, DOI, title, authors, year, venue, country or affiliation, problem area in HPC, AI/ML technique, input data type, output or decision type, research type, evaluation type, HPC environment, metrics, main contribution, main result, limitations, include decision, and notes. Problem area in HPC served as the main grouping dimension in the synthesis.

12. Critical appraisal of individual sources of evidence



13. Synthesis of results

Included studies were classified across six main axes: problem area, AI/ML technique, research type, evaluation type, HPC environment, and metrics. The synthesis was primarily descriptive and aimed to identify concentrations of research activity, dominant methods, evaluation patterns, and underexplored areas. Problem area in HPC was used as the main dimension for organizing tables and comparisons.

14. Selection of sources of evidence - results



15. Characteristics of sources of evidence



16. Critical appraisal within sources of evidence



17. Results of individual sources of evidence



18. Synthesis of results - results section



19. Summary of evidence



20. Limitations

This review is limited by the chosen time window, the selected databases, and the variability of terminology used across HPC and AI/ML publications. Some relevant studies may not be captured by database search alone, especially when authors use domain-specific or nonstandard terminology. Although the query was validated on known relevant papers and complemented with snowballing, the final corpus may still underrepresent some subareas.

21. Conclusions

This scoping review is intended to provide a structured overview of how AI and ML are currently used to address internal HPC problems. By mapping problem areas, algorithm families, evaluation strategies, environments, and metrics, the study aims to clarify the current state of the field and support future comparative and more focused review efforts.

22. Funding

