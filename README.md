# TCPRoutingTest

```sh
git clone git@github.com:miclip/TCPRoutingTest.git

# update route in manifest.yml
cd ./TCPRoutingTest/TCPRoutingServer
dotnet publish -r linux-64 
cf push
# wait for app to start, writes to log Waiting for connection

# Update port and IP for foundation in ./TCPRoutingClient/Program.cs
cd ../TCPRoutingClient
dotnet run 
```
