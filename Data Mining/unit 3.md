# Data Mining

---

- KDD versus data mining
- Stages of the Data Mining Process
- Task primitives
- Data Mining Techniques
- Data mining knowledge representation
- Data mining query languages
- Integration of a Data Mining System with a Data Warehouse
- Issues
- Data preprocessing
- Data cleaning
- Data transformation
- Feature selection
- Dimensionality reduction
- Discretization and generating concept hierarchies
- Mining frequent patterns
- Association
- correlation.

---

### Part A

- [ ] List the task primitives in the knowledge discovery process
  > [!info]- Ans
  >
  > - data cleaning
  > - integration
  > - selection
  > - transformation
  > - mining
  > - pattern evaluation
  > - knowledge presentation
- [ ] why is feature selection essential in data mining
  > [!info]- Ans
  > to identify and choose most relevant features in dataset
- [ ] define pattern evaluation
  > [!info]- Ans
  > identifying strictly increasing patterns representing knowledge based on the given measure

---

### Part B

- [ ] outline few of the knowledge representation techniques
  > [!note]- Notes
  >
  > - logical (predictive logic)
  > - sematic networks (graphical structure)
  > - frame (structured data w/ slots & fillers)
  > - rule based (conitional statements)
- [ ] explain the bining and entropy based data discretization
  > [!note]- Notes
  > method of converting huge number of data into smaller one
  >
  > - binning
  >   - equal width binning
  >   - equal frequency binning
  > - Entrophy based
- [ ] show how do you integrated data mining system with a data warehouse
  > [!note]- Notes
  >
  > - data extraction
  > - model development
  > - storing and reporting
- [ ] explain the methods of concept hierarchy generation for numeric data
  > [!note]- Notes
  >
  > - bining
  > - clustering
  > - range based

### Part C

- [ ] summarize the stages in KDD process with suitable examples

  > [!info]- Ans
  > [KDD process](https://www.geeksforgeeks.org/kdd-process-in-data-mining/)

  > [!note]- Notes
  > ![[img/kdd.png]]
  > - data cleaning
  > - data integration
  > 	- mitigation
  > 	- synchronization
  > 	- ETL
  > - data selection
  > 	- select relevent data by following
  > 		- neural network
  > 		- decision trees
  > 		- naive bayes
  > 		- clustering
  > 		- regression
  > - data transformation
  > 	- data mapping
  > 	- code generation
  > - data mining
  > 	- data to patterns
  > 		- classification
  > 		- characterization
  > - pattern evaluation
  > - knowledge representation

- [ ] illustrate apriori algorithm to find associations in frequent itemset
  > [!info]- Ans
  > [Apriori algorithm](https://www.geeksforgeeks.org/apriori-algorithm/)
  
  >[!note]- Note
  >```
  >All  subsets of frequent itemset must be frequent
  >if an itemset is infrequent, all its superset will be infrequent
  >```
  >`confidence(A -> B) = supp(A U B) / supp(A)`
