---
title: "SystemTimeInterruptMonitor.IsInterruptionRequested"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SystemTimeInterruptMonitor 属性。此实现仅检查从启动此监视器到现在的耗时是否大于用户指定的限制"
type: docs
url: /zh/net/aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/
---
## SystemTimeInterruptMonitor.IsInterruptionRequested property

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

    public class SystemTimeInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 创建 SystemTimeInterruptMonitor 的实例
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
            
            // 以 5 秒的时间限制开始监视
            monitor.StartMonitor(5000);

            // 显示初始 IsInterruptionRequested 值
            Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // 模拟长时间运行的操作
            Console.WriteLine("Starting long operation...");
            for (int i = 0; i < 100000; i++)
            {
                worksheet.Cells[i, 0].Value = i;
                
                // 检查是否请求了中断
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine("Operation interrupted after time limit!");
                    break;
                }
            }

            // 显示最终 IsInterruptionRequested 值
            Console.WriteLine("Final IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // 保存结果
            workbook.Save("PropertyIsInterruptionRequestedDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


