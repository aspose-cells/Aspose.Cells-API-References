---
title: "ThreadInterruptMonitor.TerminateWithoutException"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ThreadInterruptMonitor 属性。参见 TerminateWithoutException。此属性由用户在构造该监视器实例时指定。"
type: docs
url: /zh/net/aspose.cells/threadinterruptmonitor/terminatewithoutexception/
---
## ThreadInterruptMonitor.TerminateWithoutException property

参见 [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/)。此属性由用户在构造此监视器实例时指定。

```csharp
public override bool TerminateWithoutException { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建一个 ThreadInterruptMonitor 实例，并设置初始的 TerminateWithoutException 值
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            
            // 显示该属性的当前值
            Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);

            // 开始监控，限制为 5 秒
            monitor.StartMonitor(5000);

            // 演示可能被中断的处理过程
            try
            {
                for (int i = 0; i < 100000; i++)
                {
                    // 模拟长时间处理
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine("Processing was interrupted");
                        break;
                    }
                    worksheet.Cells[i, 0].Value = "Value " + i;
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception occurred: " + ex.Message);
            }
            finally
            {
                monitor.FinishMonitor();
            }

            // 创建另一个监视器，并将 TerminateWithoutException 设置为 true
            ThreadInterruptMonitor silentMonitor = new ThreadInterruptMonitor(true);
            Console.WriteLine("\nNew monitor TerminateWithoutException value: " + silentMonitor.TerminateWithoutException);

            // 保存结果
            workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


