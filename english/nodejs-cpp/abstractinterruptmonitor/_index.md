---
title: AbstractInterruptMonitor
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Monitor for interruption requests in all timeconsuming operations.
type: docs
url: /nodejs-cpp/abstractinterruptmonitor/
---

## AbstractInterruptMonitor class

Monitor for interruption requests in all time-consuming operations.

```javascript
abstract class AbstractInterruptMonitor;
```


## Methods

| Method | Description |
| --- | --- |
| abstract [isInterruptionRequested()](#isInterruptionRequested--)| Indicates whether interruption is requested for current operation. If true then current operation will be interrupted. Implementation should perform fast and efficient check here, otherwise it may become another bottleneck for the procedure. |
| abstract [getTerminateWithoutException()](#getTerminateWithoutException--)| When procedure is interrupted, whether terminate the procedure quietly or throw an Exception. Default is false, that is, when [IsInterruptionRequested](../isinterruptionrequested/) is true, a [CellsException](../cellsexception/) with code [ExceptionType.Interrupted](../exceptiontype.interrupted/) will be thrown. |


### isInterruptionRequested() {#isInterruptionRequested--}

Indicates whether interruption is requested for current operation. If true then current operation will be interrupted. Implementation should perform fast and efficient check here, otherwise it may become another bottleneck for the procedure.

```javascript
abstract isInterruptionRequested() : boolean;
```


### getTerminateWithoutException() {#getTerminateWithoutException--}

When procedure is interrupted, whether terminate the procedure quietly or throw an Exception. Default is false, that is, when [IsInterruptionRequested](../isinterruptionrequested/) is true, a [CellsException](../cellsexception/) with code [ExceptionType.Interrupted](../exceptiontype.interrupted/) will be thrown.

```javascript
abstract getTerminateWithoutException() : boolean;
```



