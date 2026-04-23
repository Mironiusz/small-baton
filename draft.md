1. Title

AI and Machine Learning Inside HPC: A Scoping Review

2. Structured summary

This scoping review looks at how AI and ML are used inside HPC systems to solve practical problems such as scheduling, resource allocation, workload prediction, performance modeling, anomaly detection, fault prediction, resilience, energy optimization, autotuning, runtime optimization, and code optimization. We searched four major databases, screened the results, and grouped the included studies by problem area, AI/ML technique, evaluation style, HPC environment, and metrics. The goal is to show where the field is active, which methods are popular, and where the biggest gaps still are.

3. Rationale

AI and ML are showing up more and more often in HPC research, but the field is scattered across different communities and venues. That makes it hard for practitioners to quickly see what is actually being studied, what seems promising, and what is still missing. A scoping review fits this goal well because we want a broad map of the area, not a narrow comparison of one specific technique.

4. Objectives

This review answers four questions: (RQ1) What AI/ML application areas in HPC are described in the literature? (RQ2) Which AI/ML algorithms are used in these areas? (RQ3) Which algorithms are currently reported as the most effective? (RQ4) What HPC environments and evaluation metrics are used to assess these approaches?

5. Protocol and registration

Before starting the review, we prepared a simple protocol covering the study scope, research questions, databases, search strings, eligibility rules, screening process, extraction form, and decision log. The protocol was used internally and was not formally registered.

6. Eligibility criteria

We included papers where AI or ML was used to solve a problem inside HPC, such as scheduling, resource allocation, workload prediction, performance prediction or modeling, anomaly detection, fault prediction, resilience, energy optimization, autotuning, runtime optimization, or HPC-focused code optimization. We excluded papers where HPC was only used to train AI models, where the topic was general AI for science without an HPC systems problem, where no real AI/ML method was present, or where the publication was only a tool description, keynote, editorial, or short poster without a clear method. We also excluded papers published before 2020.

7. Information sources

The core search was run in Scopus, Web of Science Core Collection, IEEE Xplore, and ACM Digital Library. We also allowed follow-up search through backward snowballing, forward snowballing, and manual checking of selected venues when needed.

8. Search

The search strategy was built from three groups of terms: AI/ML terms, HPC terms, and HPC problem terms. We prepared both a broad query and a narrower one, then adapted the syntax to each database. In practice, this meant searching titles, abstracts, keywords, metadata, and index terms depending on the platform.

9. Selection of sources of evidence

Records from all databases were exported, merged, and deduplicated. We then screened titles and abstracts and assigned one of three decisions: Include, Exclude, or Uncertain, with Uncertain treated as Exclude at this stage. A paper was included only if it clearly dealt with HPC, used AI/ML, and applied AI/ML to an operational, system-level, or optimization problem inside HPC. After that, the initial set was extended through backward and forward snowballing.

10. Data charting process

We used a structured extraction sheet to collect the same information from every included paper. The sheet covered bibliographic data, classification tags, evaluation details, and short notes about contributions, results, and limitations. LLMs were used only as a helper for summarization and draft extraction, and every generated output was checked by a human.

11. Data items

For each paper, we collected source type, database origin, DOI, title, authors, year, venue, country or affiliation, problem area in HPC, AI/ML technique, input data type, output or decision type, research type, evaluation type, HPC environment, metrics, main contribution, main result, limitations, include decision, and notes. The main grouping dimension in the analysis was the problem area in HPC.

12. Critical appraisal of individual sources of evidence



13. Synthesis of results

The included papers were grouped along six main axes: problem area, AI/ML technique, research type, evaluation type, HPC environment, and metrics. The synthesis was descriptive rather than statistical. The main goal was to show where research activity is concentrated, which approaches show up most often, and which parts of the field still look thin.

14. Selection of sources of evidence - results



15. Characteristics of sources of evidence



16. Critical appraisal within sources of evidence



17. Results of individual sources of evidence



18. Synthesis of results - results section



19. Summary of evidence



20. Limitations

This review has a few practical limits. It only covers papers from 2020 onward, it focuses on four main databases, and it depends on search terms in a field where naming is not always consistent. Even with query refinement and snowballing, some relevant studies may still have been missed.

21. Conclusions

This review aims to give a clear and practical overview of how AI and ML are being used inside modern HPC systems. By organizing the literature around real HPC problems, methods, environments, and evaluation practices, it should make the field easier to navigate for both researchers and software practitioners.

22. Funding

