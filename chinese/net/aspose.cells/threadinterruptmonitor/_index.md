---
title: "类 ThreadInterruptMonitor"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.ThreadInterruptMonitor 类。通过启动另一个线程，在睡眠用户指定的限制后要求中断，实现了 AbstractInterruptMonitor 的简单实现。"
type: docs
url: /zh/net/aspose.cells/threadinterruptmonitor/
---
## ThreadInterruptMonitor class

通过启动另一个线程，在睡眠用户指定的限制后要求中断，实现了 [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) 的简单实现。

```csharp
public class ThreadInterruptMonitor : AbstractInterruptMonitor
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [ThreadInterruptMonitor](threadinterruptmonitor/)(bool) | 构造一个中断监视器。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/threadinterruptmonitor/isinterruptionrequested/) { get; } | 此实现仅检查从启动此监视器到现在的耗时是否大于用户指定的限制。 |
| override [TerminateWithoutException](../../aspose.cells/threadinterruptmonitor/terminatewithoutexception/) { get; } | 参见 [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/)。此属性由用户在构造此监视器实例时指定。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [FinishMonitor](../../aspose.cells/threadinterruptmonitor/finishmonitor/)() | 完成对单个过程的监视。 |
| [StartMonitor](../../aspose.cells/threadinterruptmonitor/startmonitor/)(int) | 使用指定的时间限制启动监视器。用于计算耗时的起始时间就是调用此方法的时刻，因此需要监视的过程应在此调用后立即开始。 |

### 备注

一个监视器实例可以重复使用，只要按顺序监视每个过程。它不应在多线程中同时监视多个过程。

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadInterruptMonitorDemo
    {
        public static void ThreadInterruptMonitorExample()
        {
            // 创建 ThreadInterruptMonitor 实例，并将 terminateWithoutException 设置为 false
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // 创建 LoadOptions 并将 InterruptMonitor 设置为刚创建的监视器
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // 以 1000 毫秒（1 秒）的时间限制启动监视器
            monitor.StartMonitor(1000);

            try
            {
                // 使用指定的 LoadOptions 加载工作簿
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // 完成加载过程的监视器
                monitor.FinishMonitor();

                // 再次启动监视器，新的时间限制为 1500 毫秒（1.5 秒）
                monitor.StartMonitor(1500);

                // 保存工作簿
                wb.Save("result.xlsx");

                // 完成保存过程的监视器
                monitor.FinishMonitor();
            }
            catch (Exception ex)
            {
                Console.WriteLine("An exception occurred: " + ex.Message);
            }
        }
    }
}
```

### 另请参见

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


