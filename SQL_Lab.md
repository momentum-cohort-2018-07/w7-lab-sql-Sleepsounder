a The original question text
b Your final SQL query (which you must have run and validated on the included database)
b The number of results returned (if more than one)
d The specific result returned (if a single record is returned)

## The queries

1a Find all time entries.
 b  SELECT*
    FROM time_entries;

 c  500

 d


2a Find the developer who joined most recently.
 
 b  SELECT*
    FROM developers
    ORDER BY joined_on DESC
 
 c 50
 
 d "34"	"Dr. Danielle McLaughlin"	"shakira.carter@kohler.org"	"2015-07-10"	"2015-07-14        16:15:19.224045"	"2015-07-14 16:15:19.224045"


3a Find the number of projects for each client.

 b SELECT COUNT(client_id)
   FROM projects
   GROUP BY client_id;

 c 9 rows returned in 0ms

 d "3"
   "3"
   "3"
   "3"
   "6"
   "3"
   "3"
   "3"
   "3"

4a Find all time entries, and show each one's client name next to it.
 b SELECT clients.name 
   FROM time_entries 
   INNER JOIN projects on time_entries.project_id = projects.id 
   INNER JOIN clients on clients.id = projects.client_id;
 
 c 500
 
 d (500 names)



5a Find all developers in the "Ohio sheep" group.
 b
 c
 d



6a Find the total number of hours worked for each client.
 b
 c
 d



7a Find the client for whom Mrs. Lupe Schowalter (the developer) has worked the greatest number of hours.
 b
 c
 d



8a List all client names with their project names (multiple rows for one client is fine).  Make sure that clients still show up even if they have no projects.
 b
 c
 d




9a Find all developers who have written no comments.
 b
 c
 d