﻿---
title: SystemTimeInterruptMonitor
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Simple implementation of AbstractInterruptMonitor..abstractinterruptmonitor by checking and comparing current system time with user specified limit.
type: docs
url: /nodejs-cpp/systemtimeinterruptmonitor/
---

## SystemTimeInterruptMonitor class

Simple implementation of [AbstractInterruptMonitor](../abstractinterruptmonitor/) by checking and comparing current system time with user specified limit.

```javascript
class SystemTimeInterruptMonitor;
```

### Remarks
This implementation is just a simple solution for simple scenarios. It needs to frequently retrieve and check the system time so itself may have a negative impact on performance to some extent.

## Constructors

| Constructor | Description |
| --- | --- |
| [constructor(boolean)](#constructor-boolean-)| Constructs one interruption monitor. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [isInterruptionRequested](#isInterruptionRequested--)| boolean | Readonly. This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit. |
| [terminateWithoutException](#terminateWithoutException--)| boolean | Readonly. See [AbstractInterruptMonitor.TerminateWithoutException](../abstractinterruptmonitor.terminatewithoutexception/). This property is specified by user when constructing this monitor instance. |

## Methods

| Method | Description |
| --- | --- |
| [isInterruptionRequested()](#isInterruptionRequested--)| <b>@deprecated.</b> Please use the 'isInterruptionRequested' property instead. This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit. |
| [getTerminateWithoutException()](#getTerminateWithoutException--)| <b>@deprecated.</b> Please use the 'terminateWithoutException' property instead. See [AbstractInterruptMonitor.TerminateWithoutException](../abstractinterruptmonitor.terminatewithoutexception/). This property is specified by user when constructing this monitor instance. |
| [startMonitor(number)](#startMonitor-number-)| Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called, so the procedure which needs to be monitored should be started just after this call. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor(boolean) {#constructor-boolean-}

Constructs one interruption monitor.

```javascript
constructor(terminateWithoutException: boolean);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| terminateWithoutException | boolean | [AbstractInterruptMonitor.TerminateWithoutException](../abstractinterruptmonitor.terminatewithoutexception/) |

### isInterruptionRequested {#isInterruptionRequested--}

Readonly. This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit.

```javascript
isInterruptionRequested : boolean;
```


### terminateWithoutException {#terminateWithoutException--}

Readonly. See [AbstractInterruptMonitor.TerminateWithoutException](../abstractinterruptmonitor.terminatewithoutexception/). This property is specified by user when constructing this monitor instance.

```javascript
terminateWithoutException : boolean;
```


### isInterruptionRequested() {#isInterruptionRequested--}

<b>@deprecated.</b> Please use the 'isInterruptionRequested' property instead. This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit.

```javascript
isInterruptionRequested() : boolean;
```


### getTerminateWithoutException() {#getTerminateWithoutException--}

<b>@deprecated.</b> Please use the 'terminateWithoutException' property instead. See [AbstractInterruptMonitor.TerminateWithoutException](../abstractinterruptmonitor.terminatewithoutexception/). This property is specified by user when constructing this monitor instance.

```javascript
getTerminateWithoutException() : boolean;
```


### startMonitor(number) {#startMonitor-number-}

Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called, so the procedure which needs to be monitored should be started just after this call.

```javascript
startMonitor(msLimit: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| msLimit | number | time limit(ms) to require the interruption. |

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



