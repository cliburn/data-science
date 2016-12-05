# Biomedical data science programming sequence

## (1) Foundations of biomedical data science

- [Best practices for scientific computing](http://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1001745)
- Unix shell and friends
    - Unix shell
        - Files and directories
        - History and tab completion
        - Pipes and redirection
        - Looping over files
        - Creating and running shell scripts
        - Finding things
    - Regular expressions
    - Basic shell scripts
    - Remote computing
- Programming in Python
    - Using the REPL to explore Python
    - Using a text editor / IDE
    - Using libraries
    - Types and containers
    - Working with arrays
    - Reading and plotting data
    - Creating and using functions
    - Loops and conditionals
    - Defensive programming
    - Using Python from the command line
- SQL and NoSQL databases
    - Relational database concepts
    - Queries in SQL
        - Reading and sorting data
        - Filtering with where
        - Calculating new values on the fly
        - Handling missing values
        - Combining values using aggregation
        - Combining information from multiple tables using join
        - Creating, modifying, and deleting data
        - Programming with databases
    - NoSQL database examples
    - Databases and Python
- Good practices for software development
    - The [FAIR](http://www.nature.com/articles/sdata201618) (Findability, Accessibility, Interoperability and Reusability) principles
    - Writing readable code
    - Literate programming
    - Version control
        - Creating a repository
        - Recording changes to files: add, commit
        - Viewing changes: status, diff
        - Undoing changes: checkout, revert, reset
        - Ignoring files
        - Working on the web: clone, pull, push
        - Resolving conflicts
        - Where to host work, and why
    - Reproducible analysis

## (2) Data science with R

- Data manipulation
    - Tidy data
    - Using `tidyr` and `dplyr`
- Practical statistical and machine learning
    - Dimension reduction
    - Feature selection
    - Clustering
    - Classification and regression
    - Model evaluation and selection
    - Pitfalls
- Data visualization
    - Using `ggplot2`
    - Using `plot.ly`
    - Creating `shiny` applications
- Making R faster
    - Data structures, algorithms and complexity
    - Using `Rcpp` and friends
    - Multi-core computing in R
- Writing R packages for CRAN and BioConductor

## (3) Big data

- What is big data?
  - The big data bottleneck
  - Distributed computing and functional programming style
  - Introduction to cloud computing
  - Data standards, ontologies and open biomedical resources
- Storage of big data
  - NoSQL systems for data capture
  - The Hadoop ecosystem
  - Working with online/streaming data
  - Probabilisitic data structures
- Distributed data frameworks
  - The MapReduce algorithm
  - Using Spark for distributed processing
- Statistical analysis of big data
  - Scalable algorithms for data reduction/summarization
  - Scalable algorithms for unsupervised learning
  - Scalable algorithms for supervised learning

## (4) Biomedical data science case studies

- Text, NLP and EHR
    - From text to numerical features
    - Sentiment analysis
    - Topic modeling
    - Data standards for medical text processing
- Image processing
    - Working with histology images
    - Working with diagnostic images (CT/MRI)
    - Working with video images
- Genomics and other "omics"
    - Working with array data
    - Working with HTS data
    - Visualizing genomic data
    - Data standards and resources for genomics
- Space/time monitoring
  - Data from mobile platforms and GIS
  - Continuous time tracking (ICU, activity trackers)

## (A) Statistical programming with modern C++ (see detailed syllabus)

- Modern C++ for statistics
- Distributions and simulations
- Linear algebra and optimization
- Making C++ faster
