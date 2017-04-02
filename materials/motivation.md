# Why a data science track?

Direct statistical analysis is typically only possible for data that is structured and tidy, and is small enough to fit into computer memory. However, many modern biological data sets are semi-structured/unstructured and often extremely large - for example, electronic health records, time series data from wearable health trackers, medical imaging or histology slides, and genomics data from gene chip or sequencing experiments.

Dealing with these types of data requires data science skills not currently covered by the MB syllabus. In particular, mastery of the following skills would be a competitive advantage:

1. Interacting with the external world and converting data from one format to another
    1. Multiple sources
        1. Relational database
        2. NoSQL databases
        3. Spreadsheets
        4. File system
        5. Via a custom API
        6. Via web scraping
    2. Multiple formats
        1. XML
        2. JSON
        3. Tabular
        4. Specialized (e.g. laboratory assay, imaging, genomics data sets)
2. Converting unstructured or semi-structured data into structured tidy data (data munging or wrangling)
3. Data cleaning, transformation and recoding
4. Model formulation, fitting and statistical inference
    1. On large real-world biomedical data sets
    2. Proper use of machine learning pipelines
5. Model optimization
    1. Use of appropriate algorithms and data structures
    2. Use of vectorization
    3. Using compiled rather than interpreted code, which may require coding of numerical algorithms into a compiled language and interfering with a higher level language such as R
    4. Multi-core processing
6. Working with big data that cannot fit into memory
    1. Chunking
    2. Functional programming (pure functions, lazy evaluation, higher order functions)
    3. Distributed computing (remote computing and working with clusters)
    4. Working with streaming (online) data
    5. Probabilistic data structures
7. Reporting and visualization of complex data sets and analytic results
    1. Literate programming
    2. Principles of data visualization
    3. Grammar of graphics
    2. Creating interactive tools (e.g. `shiny`)
8. Construction of reproducible analysis pipelines
    1. Testing code
    2. Version control
    3. Containerization
    4. Packaging and distribution of software

The proposed sequence of four courses for the data science track will teach students the skill necessary to process large, messy biomedical data sets:

1. Foundations of biomedical data science
    - Interacting with the external world and converting data from one format to another
    - Converting unstructured or semi-structured data into structured tidy data
    - Data cleaning, transformation and recoding
    - Reporting and visualization of complex data sets and analytic results
    - Construction of reproducible analysis pipelines
2. Data science with R
    - Converting unstructured or semi-structured data into structured tidy data
    - Model formulation, fitting and statistical inference
    - Model optimization
    - Reporting and visualization of complex data sets and analytic results
    - Construction of reproducible analysis pipelines
3. Big Data
    - Overview of Big Data
    - Storage of Big Data
    - Introduction to Scala
    - Distributed data frameworks (MapReduce and Spark)
    - Statistical analysis of Big Data
4. Biomedical data science case studies
    - Woork with data sets from genomics, imaging and electronic health records
    - Data cleaning, transformation and recoding
    - Model formulation, fitting and statistical inference
    - Working with big data that cannot fit into memory
    - Reporting and visualization of complex data sets and analytic results
    - Construction of reproducible analysis pipelines
