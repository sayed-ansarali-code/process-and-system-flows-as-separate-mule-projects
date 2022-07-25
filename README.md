# process-and-system-flows-as-separate-mule-projects
It has two separate Mule projects. One having flow for process APIs, and another having Mule flow for system APIs.  System API connects to Oracle DB and get the basic user info. Process API invokes system API and concatenates firstname and lastname into field fullname and returns the response.


## Details
1. One having system API and another having process API.
1. System API connects to DB and returns csv data as "personId,firstname,lastname"
1. Process API invokes system API, converts firstname and lastname into fullname and returns response.

## Executing the project in Anypoint Studio
1. To start both the Mule projects in a single Mule container 
1. In the menu Run / Run as / Mule Application (Configure) you will see a list of open projects in the box "Mule projects to launch". 
1. Check the projects that you want to run together
1. Click on Run.
1. Access Process API at URL: http://localhost:8080/api/get-employee-data-prc
