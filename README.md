# MacAddressLookUp
The MAC Address Lookup is built using Gradle. In addition, Jib is used to  handle all the steps of packaging the Java application into a Docker image. 

To build the Java application, run command "gradle build"
To build the Docker Image, run command "gradle jibDockerBuild"
To check image name, run command "docker images" and there should be an Docker image: macaddresslookup 0.0.0-0


To execute the program,  https://macaddress.io/ apiKey is required and the MAC address, run command 
"docker run -eAPI_KEY=<apiKey> macaddresslookup:0.0.0-0 <MAC-ADDRESS>"
For example, "docker run -eAPI_KEY=at_E7TtwM4i6zZC3cIcxDBVE6kRTjSeX macaddresslookup:0.0.0-0 44:38:39:ff:ef:57"
