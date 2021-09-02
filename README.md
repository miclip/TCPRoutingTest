# TCP Routing Test

Simple TCP Listener and Client for testing TCP Routing within Tanzu Application Service

```sh
git clone git@github.com:miclip/TCPRoutingTest.git
```
Retore/build/publish server for linux runtime

```sh
cd ./TCPRoutingTest/TCPRoutingServer
dotnet publish -r linux-64 
```

Update route domain in manifest.yml
```sh
cf push
```
Wait for app to start, writes to log `Waiting for connection...` 

Update port and IP based on route for foundation in `./TCPRoutingClient/Program.cs`
```sh
cd ../TCPRoutingClient
dotnet run 
```
