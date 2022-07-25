# process-and-system-flows-as-separate-mule-projects
It has two separate Mule projects. One having flow for process APIs, and another having Mule flow for system APIs.  System API connects to Oracle DB and get the basic user info. Process API invokes system API and concatenates firstname and lastname into field fullname and returns the response.
