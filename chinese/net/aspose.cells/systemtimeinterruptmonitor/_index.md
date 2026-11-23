---
title: "类 SystemTimeInterruptMonitor"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.SystemTimeInterruptMonitor 类。通过检查和比较当前系统时间与用户指定的限制，实现 AbstractInterruptMonitor 的简易实现"
type: docs
url: /zh/net/aspose.cells/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor class

通过检查和比较当前系统时间与用户指定的限制，实现 [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) 的简易实现。

```csharp
public class SystemTimeInterruptMonitor : AbstractInterruptMonitor
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [SystemTimeInterruptMonitor](systemtimeinterruptmonitor/)(bool) | 构造一个中断监视器。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/) { get; } | 此实现仅检查从启动此监视器到现在的耗时是否大于用户指定的限制。 |
| override [TerminateWithoutException](../../aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/) { get; } | 参见 [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/)。此属性由用户在构造此监视器实例时指定。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [StartMonitor](../../aspose.cells/systemtimeinterruptmonitor/startmonitor/)(int) | 使用指定的时间限制启动监视器。用于计算耗时的起始时间就是调用此方法的时刻，因此需要监视的过程应在此调用后立即开始。 |

### 备注

此实现仅是针对简单场景的简易方案。它需要频繁获取和检查系统时间，因此在一定程度上可能对性能产生负面影响。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SystemTimeInterruptMonitorDemo
    {
        public static void SystemTimeInterruptMonitorExample()
        {
            // 创建一个 SystemTimeInterruptMonitor 实例，并将 terminateWithoutException 设置为 false
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // 创建 LoadOptions 并将 InterruptMonitor 设置为刚创建的监视器
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // 以 1000 毫秒（1 秒）的时间限制开始监视
            monitor.StartMonitor(1000);

            try
            {
                // 使用指定的 LoadOptions 加载工作簿
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // 如果加载模板文件的耗时超过一秒，则需要中断，并在此抛出异常
                // 否则，使用新的时间限制开始监视保存过程
                monitor.StartMonitor(1500); // time limit is 1.5 seconds

                // 保存工作簿
                wb.Save("SystemTimeInterruptMonitorExample.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Operation interrupted: " + ex.Message);
            }
        }
    }
}
```

### 另请参见

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


