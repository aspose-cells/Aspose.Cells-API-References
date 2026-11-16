---
title: "SystemTimeInterruptMonitor 类"
linktitle: "SystemTimeInterruptMonitor"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "SystemTimeInterruptMonitor 类。封装在 Go 中表示 systemtimeinterruptmonitor 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/systemtimeinterruptmonitor/
---

## SystemTimeInterruptMonitor class

通过检查并比较当前系统时间与用户指定的限制，提供 <see cref="AbstractInterruptMonitor"/> 的简易实现。

```go

type SystemTimeInterruptMonitor struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewSystemTimeInterruptMonitor](./newsystemtimeinterruptmonitor/) | 构造一个中断监视器。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [StartMonitor](./startmonitor/) | 使用指定的时间限制启动监视器。计算耗时的起始时间为调用此方法的时刻，因此需要监视的过程应在此调用后立即启动。 |
| [IsInterruptionRequested](./isinterruptionrequested/) | 此实现仅检查耗时（从启动此监视器到现在的时间）是否超过用户指定的限制。 |
| [GetTerminateWithoutException](./getterminatewithoutexception/) | 请参阅 AbstractInterruptMonitor.TerminateWithoutException。此属性由用户在构造此监视器实例时指定。 |
