### Extract,Load and Transform (ELT) Architrecture

![alt text](image.png)

## Data forms

without data form

![alt text](image-1.png)

- Sql development and compilation run in Dataform, and workflow execution runs in Big Query.

Structure,

![alt text](image-2.png)

Create table and view  definitions that will compile into SQL Statements

![alt text](image-3.png)

# Lab

1.Create a Dataform repository

![alt text](image-4.png)

2. Create and initialize a Dataform development workspace

![alt text](image-6.png)

![alt text](image-5.png)

3. Create a SQLX file for defining a view

![alt text](image-7.png)

```txt

config {
  type: "view"
}

SELECT
  "apples" AS fruit,
  2 AS count
UNION ALL
SELECT
  "oranges" AS fruit,
  5 AS count
UNION ALL
SELECT
  "pears" AS fruit,
  1 AS count
UNION ALL
SELECT
  "bananas" AS fruit,
  0 AS count

```

4. Create a SQLX file for table definition

create file is same process as before,

```txt

config {
  type: "table"
}

SELECT
  fruit,
  SUM(count) as count
FROM ${ref("quickstart-source")}
GROUP BY 1

```

5. Grant Dataform access to BigQuery

![alt text](image-8.png)

IAM Permissions:


