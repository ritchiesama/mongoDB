1.Download the installer from (https://www.mongodb.com/try/download/community)  
2.Install the mongo db under the direction  
3.Open cmd in the .\Mongdb\Server\4.4\bin
4.Keyin 
```cmd  
> mongod
```
If the error blow throw:

> {"t":{"$date":"2021-04-27T19:37:25.629-05:00"},"s":"E",  "c":"STORAGE",  "id":20557,   "ctx":"initandlisten","msg":"DBException in initAndListen,  
> terminating","attr":{"error":"NonExistentPath: Data directory C:\\data\\db\\ not found. Create the missing directory or specify another path   
> using (1) the --dbpath command line option, or (2) by adding the 'storage.dbPath' option in the configuration file."}}

Then we need to create a new folder at C:\data\db  

5.Re-type 
```cmd
> mongod
```
6.Open another cmd which the path same as the previous one  
7.Typing
```cmd
show dbs;
```
The following information should be shown:
>admin   0.000GB 
>config  0.000GB 
>local   0.000GB 


Create short path:  
1. Copy the path of .\Mongdb\Server\4.4\bin
2. Open Find, type Variable, open Edit the System Environment Variable
3. Open Environment Variables
4. Click the path line in the System variables
5. Click New, and Paste the path we just copied
6. Click OK on all the windows
7. Next time we can run the mongodb in the original cmd through the command
```cmd
> mongod
```
