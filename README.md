# Comparator-comparing-2-API-Response
Create a comparator that can be used to compare 2 API responses (HTTP/HTTPS)

The input to your code should be two files with millions of request URLs. Sample content for files:
Each file contains (HTTP/HTTPS) APIs separated by a new line
File1 File2
https://reqres.in/api/users/3 https://reqres.in/api/users/2
https://reqres.in/api/users/1 https://reqres.in/api/users?page=3
https://reqres.in/api/users/2 /api/unknown/2
https://reqres.in/api/users?page=2 https://reqres.in/api/users?page=2
https://reqres.in/api/users?page=1 … and so on
…. And so on
Must have
● Your compare function should be able to compare two JSON responses. [Avoid using a thirdparty
library or dependency for comparing JSONs]
● Assume that your code should be capable of comparing millions of API requests without
any memory issues. [Mandatory: Test with at least 1000 requests]
● Handle exceptions gracefully (don't terminate the program in case of exceptions)
● Print the output when responses are compared in the below format.
https://reqres.in/api/users/3 not equals https://reqres.in/api/users/1
https://reqres.in/api/users/2 equals https://reqres.in/api/users/2
https://reqres.in/api/users?page=1 equals https://reqres.in/api/users?page=1
● Please Add tests for your utility to prove the library works for different possible condition
