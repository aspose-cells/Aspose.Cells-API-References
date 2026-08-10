---
title: "SystemTimeInterruptMonitor Class"
linktitle: "SystemTimeInterruptMonitor"
articleTitle: "SystemTimeInterruptMonitor"
second_title: "Aspose.Cells for PHP via Java"
description: "Simple implementation of AbstractInterruptMonitor by checking and comparing current system time with user specified limit."
type: docs
weight: 6500
url: /php/aspose.cells/systemtimeinterruptmonitor/
---

## SystemTimeInterruptMonitor class

Simple implementation of AbstractInterruptMonitor by checking and comparing current system time with user specified limit.

## Constructors

| Name | Description |
| --- | --- |
| [SystemTimeInterruptMonitor](#constructor) | Constructs one interruption monitor. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IsInterruptionRequested](#isinterruptionrequested) | boolean | This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than u |
| [TerminateWithoutException](#terminatewithoutexception) | boolean | See TerminateWithoutException . This property is specified by user when constructing this monitor instance. |

## Methods

| Name | Description |
| --- | --- |
| [startMonitor](#startmonitor) | Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is call |

### SystemTimeInterruptMonitor(terminateWithoutException) {#constructor}

Constructs one interruption monitor.

| Parameter | Type | Description |
| --- | --- | --- |
| terminateWithoutException | boolean | TerminateWithoutException |

### SystemTimeInterruptMonitor.IsInterruptionRequested property {#isinterruptionrequested}

This implementation just checks whether the time cost(from the time when starting this monitor to now) is greater than user specified limit.

**Type:** boolean

### SystemTimeInterruptMonitor.TerminateWithoutException property {#terminatewithoutexception}

See TerminateWithoutException . This property is specified by user when constructing this monitor instance.

**Type:** boolean

### startMonitor(msLimit) {#startmonitor}

Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called, so the procedure which needs to be monitored should be started just after this call.

| Parameter | Type | Description |
| --- | --- | --- |
| msLimit | Number | time limit(ms) to require the interruption. |
