---
title: "ThreadInterruptMonitor.ThreadInterruptMonitor"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ThreadInterruptMonitor 构造函数。构造一个中断监视器"
type: docs
url: /zh/net/aspose.cells/threadinterruptmonitor/threadinterruptmonitor/
---
## ThreadInterruptMonitor constructor

构造一个中断监视器。

```csharp
public ThreadInterruptMonitor(bool terminateWithoutException)
```

| 参数 | 类型 | 描述 |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            
            // 创建一个 ThreadInterruptMonitor，并将 throwOnInterrupted 设置为 false
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            workbook.InterruptMonitor = monitor;
            
            // 设置一个短时间限制（100 毫秒）用于演示
            int timeLimit = 100;
            monitor.StartMonitor(timeLimit);

            try
            {
                // 执行一个长时间操作（将被中断）
                for (int i = 0; i < 100000; i++)
                {
                    workbook.Worksheets[0].Cells[i % 100, i / 100].PutValue(i);
                }
                
                Console.WriteLine("Operation completed without interruption");
            }
            catch (CellsException e)
            {
                if (e.Code == ExceptionType.Interrupted)
                {
                    Console.WriteLine("Operation was successfully interrupted");
                }
                else
                {
                    Console.WriteLine("Error occurred: " + e.Message);
                }
            }
        }
    }
}
```

### 另请参见

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


