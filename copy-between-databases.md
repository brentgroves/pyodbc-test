https://thepythonguru.com/fetching-records-using-fetchone-and-fetchmany/

https://code.google.com/archive/p/pyodbc/wikis/Cursor.wiki

If using select/insert then it is better to insert in batches of 500 records or so.

fetchmany
cursor.fetchmany([size=cursor.arraysize]) --> list

Returns a list of remaining rows, containing no more than size rows, used to process results in chunks. The list will be empty when there are no more rows.

The default for cursor.arraysize is 1 which is no different than calling fetchone().

A ProgrammingError exception is raised if no SQL has been executed or if it did not return a result set (e.g. was not a SELECT statement).

