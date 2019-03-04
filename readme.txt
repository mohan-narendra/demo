spring-boot app which determines if two cities are connected. Two cities are considered connected if there’s a series of roads that can be traveled from one city to another. 
Note: I have implemented graph traversal using Breadth First method. I have tested code with limited set of data .

Coding exercise Write a program in Java which determines if two cities are connected.Two cities are considered connected if there’s a series of roads that can be traveled from one city to another. List of roads is available in a file.File contains a list of city pairs (one pair per line, comma separated), which indicates that there’s a road between those cities. 

It will be deployed as a spring-boot app and expose one endpoint: 
http://localhost:8080/connected?origin=city1&destination=city2

Your program should respond with ‘yes’ if city1 is connected to city2, ’no’ if city1 is not connected to city2.
Any unexpected input should result in a ’no’ response.
Example: 

city.txt content is: 
Boston, New York
Philadelphia, Newark
Newark, Boston
Trenton, Albany

http://localhost:8080/connected?origin=Boston&destination=Newark
Should return yes
http://localhost:8080/connected?origin=Boston&destination=Philadelphia
Should return yes
http://localhost:8080/connected?origin=Philadelphia&destination=Albany
Should return no

I added the swagger documentation file to in project root folder to test the /connected  endpoint

Thanks,
Narendra 