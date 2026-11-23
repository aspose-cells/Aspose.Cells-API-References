---
title: "SystemTimeInterruptMonitor.TerminateWithoutException"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SystemTimeInterruptMonitor 属性。参见 TerminateWithoutException。此属性由用户在构造此监视器实例时指定"
type: docs
url: /zh/net/aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/
---
## SystemTimeInterruptMonitor.TerminateWithoutException property

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

    public class SystemTimeInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // 使用初始 TerminateWithoutException 值创建 SystemTimeInterruptMonitor 的实例
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // 显示 TerminateWithoutException 属性的当前值
            Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);

            // 以 1000 毫秒的时间限制开始监视
            monitor.StartMonitor(1000);

            // 通过尝试长时间操作演示 TerminateWithoutException 的效果
            try
            {
                // 模拟可能超出时间限制的长时间操作
                for (int i = 0; i < 100000; i++)
                {
                    worksheet.Cells[i, 0].Value = i;
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine("Operation interrupted by monitor");
                        break;
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception caught: " + ex.Message);
            }

            // 创建另一个监视器，并将 TerminateWithoutException 设置为 true
            SystemTimeInterruptMonitor monitorNoException = new SystemTimeInterruptMonitor(true);
            Console.WriteLine("New monitor TerminateWithoutException value: " + monitorNoException.TerminateWithoutException);

            // 保存工作簿
            workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


