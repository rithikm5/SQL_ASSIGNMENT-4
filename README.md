# SQL_ASSIGNMENT-4
# Write a query to display / print only the last name in all caps from "Sanjay Kumar" with padding of "%"
# input in query: Sanjay Kumar
# output display: %%KUMAR%%

SELECT CONCAT(
         '%%',
         UPPER(SUBSTRING_INDEX('Sanjay Kumar', ' ', -1)),
         '%%'
       ) AS Output;
