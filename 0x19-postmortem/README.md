
![Cod](/c/Users/Lucy/Desktop/ALX/alx-system_engineering-devops/0x19-postmortem/web.png)

# Mastodon server requests failure report

Last week, it was reported that the Mastodon server was returning 500 Error on all requests made on the platform routes, all the services were down. 90% of 
the users were affected. The root cause was the due to increase in traffic.

## Timeline
The error was realized on November 6, 2022 1200 hours (East Africa Time).The engineers increased the number of database connections and worker processses 
to help clear backlogs and background tasks.

## Root cause and resolution
The COD Server is served by 2 ubuntu cloud servers. The master server  was connected to serve all requests, and it stopped functioning due to 
memory outage as a results of so many requests because during a previous test, the client server  
was disconnected temporarily for testing and was not connected to the load balancer afterwards.

## Measures against such problem in future
* Choose the best loadbalancing algorithm for your programs
* Always keep an eye on your servers to ensure they are running properly
* Have extra back-up servers to prevent your program from completely going offline during an issue.
