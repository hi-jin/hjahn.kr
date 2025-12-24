---
{"publish":true,"created":"2025-12-24T15:58:37.415+09:00","modified":"2024-10-01","cssclasses":""}
---


Analyzing rejection patterns in academic papers to uncover key insights for crafting exceptional research papers

> This is a simple analysis driven by personal curiosity about “`why papers get rejected`” rather than a rigorously validated research experiment.

### TL;DR

This research project investigates the common patterns found in rejected academic papers.  
Through the analysis, I tried to uncover key insights into `why papers face rejection` and distilled essential principles for `crafting exceptional papers` that stand out to reviewers and earn acceptance.

Major rejection reasons (essential principles) are:
- Readability: How well the paper can be understood by the target audience
- Clarity: Clear presentation of ideas, methods, and results
- Contribution: Significance and novelty of the research findings
- Generalizability: Broader applicability of the research beyond specific cases
- Systematic Experimentation: Rigorous methodology and thorough validation

![[projects/attachments/Pasted image 20251224155929.png]]
> The patterns of rejected papers from OpenReview. (Searched on Google. 955 review data)

### Process 1. Crawl and refine data

![[projects/attachments/Pasted image 20251224160318.png]]
1. `Crawl rejected papers from Google`
    Using specific keywords, we can crawl only `rejected` papers from `openreview.net`.
2. `Analyze reviews`    
    I used OpenAI API (gpt-4o) to analyze reviews.  
    The model read reviews and extracted the summary.
3. `Refine data`
    I manually extracted the rejection reasons from the summaries.  
    (Not perfect..)

### Process 2. Vectorize and visualize rejection patterns

![[projects/attachments/Pasted image 20251224160400.png]]

Now we have a dataset with 955 rejection reasons.
1. `Embed rejection reasons`    
    I used OpenAI `text-embedding-3-large` to vectorize the rejection reasons.
2. `Visualize vectors`
    I used `UMAP` to reduce the dimensions, used `K-Means Clustering` to find the clusters, and visualized the rejection reasons in 2D space.

### Result (Same as the first image)

![[projects/attachments/Pasted image 20251224155929.png]]

### Insights
- `Readability`: Papers must be written in a way that is easily digestible for the target audience.
    - Proper use of technical terminology, well-structured sentences, and logical flow between sections.
    - Poor readability can obscure even groundbreaking research.
- `Clarity`: Research papers need clear presentation of ideas, methodologies, and findings.
    - Well-defined problem statements and research objectives
    - Precise description of results with appropriate visualizations
    - Logical connections between different sections
- `Contribution`: The research must make meaningful and novel contributions to the field.
    - Clear advancement over existing work
    - Novel insights or methodologies
    - Practical impact or theoretical significance
    - Addressing important gaps in current knowledge
- `Generalizability`: Research findings should have broader implications.
    - Applicability across different domains or scenarios
    - Scalability to real-world applications
    - Clear discussion of limitations and boundary conditions
    - Potential for extension to other research areas
- `Systematic Experimentation`: Research must demonstrate scientific rigor.
    - Well-designed experimental setup
    - Comprehensive ablation studies
    - Statistical validation of results
    - Comparison with baseline methods
    - Reproducible methodology
