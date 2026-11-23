---
title: "ThreadInterruptMonitor.IsInterruptionRequested"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ThreadInterruptMonitor 属性。此实现仅检查从启动监视器到现在的耗时是否超过用户指定的限制"
type: docs
url: /zh/net/aspose.cells/threadinterruptmonitor/isinterruptionrequested/
---
## ThreadInterruptMonitor.IsInterruptionRequested property

此实现仅检查从启动此监视器到现在的耗时是否大于用户指定的限制。

```csharp
public override bool IsInterruptionRequested { get; }
```

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Threading;

    public class ThreadInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建 ThreadInterruptMonitor 的实例
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(terminateWithoutException: false);

            // 开始监控，限制为 2 秒
            monitor.StartMonitor(2000);

            // 模拟长时间运行的操作
            Console.WriteLine("Starting long operation...");
            for (int i = 0; i < 100; i++)
            {
                // 检查是否请求了中断
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine("Operation was interrupted!");
                    break;
                }

                // 模拟工作
                Thread.Sleep(100);
                worksheet.Cells[i, 0].Value = $"Processed row {i}";
                Console.WriteLine($"Processed row {i}");
            }

            // 结束监控
            monitor.FinishMonitor();

            // 保存结果
            workbook.Save("ThreadInterruptionDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


