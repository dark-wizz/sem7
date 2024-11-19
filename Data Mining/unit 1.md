# Evolution of Decision Support Systems

---

- Data warehousing Components
- Building a Data warehouse
- Data Warehouse and DBMS
- Data marts
- Metadata
- Multidimensional data model
- OLAP Vs OLTP - OLAP operations
- Data cubes
- Schemas for Multidimensional Database
  - Stars
  - Snowflakes and Fact constellations.

---

### Part A

- [ ] define data warehouse
  > [!info]- Ans
  > A centralised system that stores and analyze data from various sources
- [ ] what does the term metadata mean
  > [!info]- Ans
  > Metadata is defined as the data providing information about one or more aspects of the data such as structure, contents or other characteristics
- [ ] name the schemes for multi dimensional database
  > [!info]- Ans
  >
  > - Star schema
  > - Snowflake schema
  > - Galaxy schema
- [ ] why is metadata essential
  > [!info]- Ans
  > Meta data is essential for understanding managing, and using data effectively

---

- [ ] define data acquisition
  > [!info]- Ans
  > DAQ is the process of collecting and converting real-world physical data into digital values that can be analyzed by computer

### Part B

- [ ] define data marts? explain how data mart is structured
  > [!note]- Notes
  >
  > - storage components
  > - subset of data warehouse
  > - focused on one particular function
  >
  > ##### Data warehouse structure
  >
  > - dependent
  > - independent
  > - hybrid
- [ ] list the significant aspects of OLAP and OLTP
  > [!note]- Notes
  > | OLAP | OTAP |
  > | ---- | ---- |
  > | online analytical processing | online transactional processing |
  > | query management system | modyfying system |
  > | use of warehouse | use of DBMS |
  > | subject oriented | application oriented |
  > | used for analytics, decision making | business tasks |
  > | large amount of data | small |
- [ ] what is star schema
- [ ] recall data cubes with suitable example
  > [!note]- Notes
  > Grouping data in a multidimensional matrix
  > ![[img/datacube.png]]

### Part C

- [ ] describe schemas in data warehouse

  > [!info]- Ans
  > [Schemas](https://www.softwareag.com/en_corporate/blog/streamsets/schemas-data-warehouses-star-galaxy-snowflake.html) > [!note]- Notes

  > [!note]- Notes
  >
  > ###### fact table
  >
  > stores primary keys of dimensional table as foreign keys
  > ![[img/fact_table.png]]
  >
  > ###### dimensional table
  >
  > not joined together, joined via associations
  > ![[img/dim_table.png]]
  >
  > ###### star schema
  >
  > - dim table not connected directly
  > - denormalized
  > - quick query response
  > - each dim maps to one dim table
  > - one face table only
  >   ![[img/star_schema.png]]
  >
  > ###### Snowflake schema
  >
  > - dim table joined to other dim table
  > - one fact table only
  > - normalised
  > - low disk space
  >   ![[img/snow_schema.png]]
  >
  > ###### galaxy schema
  >
  > - zero redundancy
  > - normalized
  > - high quality and accuracy
  >   ![[img/galaxy_schema.png]]

- [ ] explain the data warehousing components
  > [!note]- Notes
  > ![[img/dw_comp.png]]
  >
  > - source data components
  >   - Production data
  >   - Internal data
  >   - Archived data
  >   - External data
  > - Data staging comp
  >   - Extraction
  >   - Transformation
  >   - Loading
  > - Data storage comp
  > - Information delivery comp
  > - Metadata comp
  > - Data marts
  > - Management and control comp
