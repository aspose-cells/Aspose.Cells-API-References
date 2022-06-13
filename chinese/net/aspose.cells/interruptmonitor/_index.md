---
title: InterruptMonitor
second_title: Aspose.Cells for .NET API 参考
description: 代表所有关于中断的操作符
type: docs
weight: 3910
url: /zh/net/aspose.cells/interruptmonitor/
---
## InterruptMonitor class

代表所有关于中断的操作符。

```csharp
public class InterruptMonitor : AbstractInterruptMonitor
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [InterruptMonitor](interruptmonitor)() | 默认构造函数。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/interruptmonitor/isinterruptionrequested) { get; } | 将监视器标记为请求中断 |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception) { get; } | 当程序被中断时，是安静地终止程序还是抛出异常。 默认为假，即当[`IsInterruptionRequested`](../abstractinterruptmonitor/isinterruptionrequested)为真时， a[`CellsException`](../cellsexception)代码Interrupted将被抛出。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Interrupt](../../aspose.cells/interruptmonitor/interrupt)() | 中断当前操作符。 |

### 也可以看看

* class [AbstractInterruptMonitor](../abstractinterruptmonitor)
* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->