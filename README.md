# PowerBI-M-Language-REST-API-Connection

This project contains some useful code sample for connecting your data to PowerBI/ Power Query in Power BI Data Flow via REST APIs.

There are two diffeent files showing the connection method for two different type APIS:

A) "Auth 1.0" connects API with only one TOKEN KEY. (Not scure, and sometimes failed)

B) "Auth 2.0" connects API with a dynamic token:
  1. You need use your CONSUMER KEY and CONSUMER SECRET to access the dynamic Token
  2. Then you should use current TOKEN to access the link of data.
  
  
* In the step of accessing and loading data, I strongly encourage you to add '&limit=xxxxxx' at the end of your API link to limit the row of data and optimize the loading speed.
* In some cases, if your original data table has several pages, you should add '?pageNumber=xx' at the end of your API link to load each page seperately.
