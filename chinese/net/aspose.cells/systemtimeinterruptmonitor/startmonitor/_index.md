---
title: "SystemTimeInterruptMonitor.StartMonitor"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SystemTimeInterruptMonitor 方法。使用指定的时间限制启动监视器。用于计算耗时的开始时间就是调用此方法的时刻，因此需要被监视的过程应在此调用后立即开始。"
type: docs
url: /zh/net/aspose.cells/systemtimeinterruptmonitor/startmonitor/
---
## SystemTimeInterruptMonitor.StartMonitor method

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
    public class SystemTimeInterruptMonitorMethodStartMonitorWithInt32Demo
    {
        public static void Run()
        {
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            monitor.StartMonitor(1000); // 1 second time limit

            try
            {
                Workbook wb = new Workbook("Large.xlsx", lopts);
                monitor.StartMonitor(1500); // 1.5 second time limit
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

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


