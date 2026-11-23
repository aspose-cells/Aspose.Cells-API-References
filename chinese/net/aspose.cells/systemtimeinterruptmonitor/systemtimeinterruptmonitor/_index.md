---
title: "SystemTimeInterruptMonitor.SystemTimeInterruptMonitor"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "SystemTimeInterruptMonitor 构造函数。构造一个中断监视器"
type: docs
url: /zh/net/aspose.cells/systemtimeinterruptmonitor/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor constructor

构造一个中断监视器。

```csharp
public SystemTimeInterruptMonitor(bool terminateWithoutException)
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
    public class SystemTimeInterruptMonitorMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // 创建一个实例，将 terminateWithoutException 设置为 false
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // 使用监视器设置加载选项
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // 以 1 秒的时间限制开始监视
            monitor.StartMonitor(1000);

            try
            {
                // 尝试加载工作簿
                Workbook wb = new Workbook("sample.xlsx", lopts);

                // 为保存操作重置监视器，时间限制为 1.5 秒
                monitor.StartMonitor(1500);
                wb.Save("output.xlsx");
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


