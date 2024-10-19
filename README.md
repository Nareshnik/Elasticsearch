 Elasticsearch

 # Employee Data Indexing project
This project involves working with Elasticsearch to index employee data. The objective is to perform various operations like creating collections, indexing data, searching by specific columns, and retrieving employee counts.

## Installation Instructions
1. **Read about Elasticsearch:** Familiarize yourself with the basics by reading the [Getting Started with Elasticsearch](https://www.elastic.co/guide/en/elasticsearch/reference/current/getting-started.html).
2. **Install Elasticsearch:** Follow the official installation guide to set up Elasticsearch on your local machine.
3. **Download Employee Dataset:** Obtain the employee data set from [Kaggle](https://www.kaggle.com/datasets/williamlucas0/employee-sample-data).

## Function Definitions
The following functions were implemented as part of the assignment:
- `createCollection(p_collection_name)`
- `indexData(p_collection_name, p_exclude_column)`
- `searchByColumn(p_collection_name, p_column_name, p_column_value)`
- `getEmpCount(p_collection_name)`
- `delEmpById(p_collection_name, p_employee_id)`
- `getDepFacet(p_collection_name)`

## Function Executions
The following sequences of function calls were executed:
1. **Create Collections:**
   - `createCollection('hash_<Your Name>')`
   - `createCollection('hash_<Your Phone last four digits>')`
2. **Get Employee Count:**
   - `getEmpCount('hash_<Your Name>')`
3. **Index Data:**
   - `indexData('hash_<Your Name>', 'Department')`
   - `indexData('hash_<Your Phone last four digits>', 'Gender')`
4. **Delete Employee:**
   - `delEmpById('hash_<Your Name>', 'E02003')`
5. **Search Operations:**
   - `searchByColumn('hash_<Your Name>', 'Department', 'IT')`
   - `searchByColumn('hash_<Your Name>', 'Gender', 'Male')`
   - `searchByColumn('hash_<Your Phone last four digits>', 'Department', 'IT')`
6. **Get Department Facets:**
   - `getDepFacet('hash_<Your Name>')`
   - `getDepFacet('hash_<Your Phone last four digits>')`

## Results
- Employee count before and after deletion.
- Data indexed into collections.
- Search results based on specified criteria.
- Department counts retrieved from the collections.

