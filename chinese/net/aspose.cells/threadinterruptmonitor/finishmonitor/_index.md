---
title: "ThreadInterruptMonitor.FinishMonitor"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "ThreadInterruptMonitor 方法。结束对单个过程的监控"
type: docs
url: /zh/net/aspose.cells/threadinterruptmonitor/finishmonitor/
---
## ThreadInterruptMonitor.FinishMonitor method

完成对单个过程的监视。

```csharp
public void FinishMonitor()
```

### 备注

在受监控的过程结束后调用此方法可以提前释放监视线程，尤其是在该过程未被中断的情况下（该过程的耗时小于指定的时间限制）。

### 示例

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodFinishMonitorDemo
    {
        public static void Run()
        {
            // 创建 ThreadInterruptMonitor 的实例
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // 创建 LoadOptions 并设置 InterruptMonitor
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // 开始监控，超时为 1 秒
            monitor.StartMonitor(1000);

            try
            {
                // 模拟长时间运行的操作
                for (int i = 0; i < 5; i++)
                {
                    System.Threading.Thread.Sleep(200);
                    Console.WriteLine($"Processing step {i + 1}");
                }

                // 结束对该操作的监控
                monitor.FinishMonitor();
                Console.WriteLine("Operation completed successfully");
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

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


