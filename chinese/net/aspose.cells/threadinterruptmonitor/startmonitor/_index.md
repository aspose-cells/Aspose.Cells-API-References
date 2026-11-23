---
title: "ThreadInterruptMonitor.StartMonitor"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ThreadInterruptMonitor 方法。使用指定的时间限制启动监视器。用于计算耗时的开始时间是在调用此方法时刻，因此需要监控的过程应在此调用后立即启动。"
type: docs
url: /zh/net/aspose.cells/threadinterruptmonitor/startmonitor/
---
## ThreadInterruptMonitor.StartMonitor method

使用指定的时间限制启动监视器。用于计算耗时的起始时间就是调用此方法的时刻，因此需要监视的过程应在此调用后立即开始。

```csharp
public void StartMonitor(int msLimit)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| msLimit | Int32 | 要求中断的时间限制（毫秒） |

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodStartMonitorWithInt32Demo
    {
        public static void Run()
        {
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            monitor.StartMonitor(1000);

            try
            {
                Workbook wb = new Workbook("Large.xlsx", lopts);
                monitor.FinishMonitor();

                monitor.StartMonitor(1500);
                wb.Save("result.xlsx");
                monitor.FinishMonitor();
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception: " + ex.Message);
            }
        }
    }
}
```

### 另请参见

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


