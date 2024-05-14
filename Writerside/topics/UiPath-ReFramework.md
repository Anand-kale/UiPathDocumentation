# UiPath ReFramework

## Overview
ReFramework is based on state machines, and by default it provides all
best practices included like logging, error handling, error screenshots, application initialization, application killing.

ReFramework Divides into four parts that are **Initialization, Get Transaction Data,
Process Transaction, End Process**.

ReFramework work with queues and without queues

* ReFramework with Queue
  - UiPath by default provides a ReFramework with queue, and it is properly configured by UiPath.
  - Prerequisites—Enable or create queue on orchestrator then specify name in UiPath Studio.
  - Basically, if we use queue, then it is straightforward to implement a process.
* ReFramework without Queue
  - UiPath by default doesn't provide a without queue support for which we need to use and datatable and datarow datatypes for implementation of ReFramework without a queue
  - We use if we want to develop a robot using ReFramework, but we need offline execution then we use.

![ReFramework](image_6.png)

* Init State
  - Here All types of initialization are done like opening and closing applications.
  - ![Init State](image_7.png)
* Get Transaction Date State
  - In this state, data will be stored in queue for each transaction.
  - ![Get Transaction Data](image_8.png)
* Process Transaction State
  - Here all executions of process will be done sequentially
  - All business logic we added here.
  - ![Process Transaction State](image_9.png)
* End Process
  - If the transaction completed there all processes, then the transaction comes here and the process gets terminated. 
  - ![End Process State](image_10.png)