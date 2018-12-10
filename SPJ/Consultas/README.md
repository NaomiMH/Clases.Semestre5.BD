# SPJ Consultas

## Simple Queries 
1.	Get all the data of all jobs (J table). 
2.	Get all the data on all jobs in London. 
3.	Get supplier numbers for suppliers (S table) who supply (SPJ table) job J1, in supplier number order. 
4.	Get all shipments (SPJ table) where the quantity is in the range 300 to 750 inclusive. 
5.	Get a list of all part-color, part-city combinations, with duplicate (color, city) eliminated. 
## Joins  
6.	Get all supplier-number, part-number, job-number triples such that the indicated supplier, part, job are in the same city. 
7.	Get all supplier-number, part-number, job-number triples such that the indicated supplier, part, job are not in the same city. 
8.	Get all supplier-number, part-number, job-number triples such that no two of the indicated supplier, part, job are in the same city. 
9.	Get part number for parts supplied (SPJ table) by a supplier in London. 
10.	Get part numbers for parts supplied by a supplier in London to a job in Paris. 
11.	Get all pairs of city names such that a supplier in the first city supplies a job in the second city. 
12.	Get part numbers for parts supplied to any job by a supplier in the same city as the job. 
13.	Get job numbers for jobs supplied by at least one supplier not in the same city. 
14.	Get all pairs of part numbers such that the same supplier supplies both the indicated parts. 
## Aggregate Functions  
15.	Get the total number of jobs supplied by supplier S1. 
16.	Get the total quantity of part P1 supplied by supplier S1. 
17.	For each part being supplied to a job, get the part number, the job number and the corresponding total quantity. 
18.	Get part numbers for parts supplied to some job in the average quantity of more than 320. 
## Special Data 
19.	Get all shipments where the quantity is non-null. 
20.	Get project numbers and cities where the city has an "o" as the second letter of its name. 
## Subqueries 
21. Get job names for jobs supplied by supplier S1.
22. Get colors for parts supplied by supplier S1.
23. Get part numbers for parts supplied to any job in London.
24. Get job numbers for jobs using at least one part available from supplier S1.
25. Get supplier numbers for suppliers supplying at least one part supplied by at least one supplier who supplies at least one red part.
26. Get supplier numbers for suppliers with status lower than that of supplier S1.
27. Get job numbers for jobs whose city is first in the alphabetic list of such cities. 
28. Get job numbers for jobs supplied with part P1 in an average quantity greater than the greatest quantity in which any part is supplied to project J1.
29. Get supplier numbers for suppliers supplying some job with part P1 in a quantity greater than the average shipment quantity of part P1 for that project.
## EXISTS  
30. Repeat Exercise 23 but use EXISTS in your solution.
31. Repeat Exercise 24 but use EXISTS in your solution.
32. Get job numbers for jobs not supplied with any red part by any London supplier.
33. Get job numbers for jobs supplied entirely by supplier S1.
34. Get part numbers for parts supplied to all jobs in London.
## UNION 
35. Construct a list of all cities in which at least one supplier, part, or job is located.
36. Show the results of the following SELECT:
SELECT P.CPLOR
FROM P
UNION
SELECT P.COLOR
FROM P;
## Upgrade Operations 
37. Change the color of all red parts to orange.
38. Delete all projects for which there are no shipments.
39. Insert a new supplier (S10) into table S. The name and city are Smith and New York, respectively; he status is yet known.
40. Construct a table containing a list of part numbers for parts that are supplied either by a London supplier or to a London Job.
41. Construct a table containing a list of job numbers for jobs that are either located in London or are supplied by a London supplier.
## Miscellaneous 
42. Get supplier names that have a letter 'e' somewhere in their name.
43. Get suppliers names which start the letters 'Bla'.
44. How many suppliers in Athens that supply red parts?
45. Delete all suppliers that never supplied a red part.
