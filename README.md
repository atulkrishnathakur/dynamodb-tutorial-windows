# How to use  DynamoDB in local machine
1. download and install java jdk https://www.oracle.com/in/java/technologies/downloads/#jdk26-windows
2. check java version
```
C:\Users\Atul Krishna Thakur>java --version
java 26.0.1 2026-04-21
Java(TM) SE Runtime Environment (build 26.0.1+8-34)
Java HotSpot(TM) 64-Bit Server VM (build 26.0.1+8-34, mixed mode, sharing)

C:\Users\Atul Krishna Thakur>
```
3. Download the dynamodb zip file from https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/DynamoDBLocal.DownloadingAndRunning.html
4. Extract the dynamodb zip file. Create a dynamodb directory in `D:\dynamodb` drive. Copy all content of extracted directory and paste in `D:\dynamodb`
5. go to `D:\dynamodb`
```
D:\>cd dynamodb
```
6. Now run the dynamodb `D:\dynamodb>java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb`
```
D:\dynamodb>java -Djava.library.path=./DynamoDBLocal_lib -jar DynamoDBLocal.jar -sharedDb
Initializing DynamoDB Local with the following configuration:
Port:   8000
InMemory:       false
Version:        3.3.0
DbPath: null
SharedDb:       true
shouldDelayTransientStatuses:   false
CorsParams:     null
```
