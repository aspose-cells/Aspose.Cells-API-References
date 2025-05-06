---
title: ThreadInterruptMonitor.StartMonitor
second_title: Aspose.Cells for .NET API Reference
description: ThreadInterruptMonitor method. Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called so the procedure which needs to be monitored should be started just after this call
type: docs
url: /net/aspose.cells/threadinterruptmonitor/startmonitor/
---
## ThreadInterruptMonitor.StartMonitor method

Starts the monitor with the specified time limit. The start time to calculate time cost is just when this method is called, so the procedure which needs to be monitored should be started just after this call.

```csharp
public void StartMonitor(int msLimit)
```

| Parameter | Type | Description |
| --- | --- | --- |
| msLimit | Int32 | time limit(ms) to require the interruption. |

### Examples

```csharp
// Called: m.StartMonitor(limit);
[Test]
        public void Method_Int32_()
        {
            for (int i = 0; i &lt; 2; i++)
            {
                long t = DateTime.Now.ToFileTimeUtc();
                Workbook wb = new Workbook();
                Model.RandomFill(wb.Worksheets[0].Cells, 5000, 20, true);
                int limit = ((int)((DateTime.Now.ToFileTimeUtc() - t) / 10000)) &gt;&gt; 2; //by test the time cost of saving is about half of that of filling
                string msg;
                if (i != 0)
                {
                    msg = &quot;SystemTimeInterruptMonitor: &quot;;
                    SystemTimeInterruptMonitor m = new SystemTimeInterruptMonitor(false);
                    wb.InterruptMonitor = m;
                    t = DateTime.Now.ToFileTimeUtc();
                    m.StartMonitor(limit);
                }
                else
                {
                    msg = &quot;ThreadInterruptMonitor: &quot;;
                    ThreadInterruptMonitor m = new ThreadInterruptMonitor(false);
                    wb.InterruptMonitor = m;
                    t = DateTime.Now.ToFileTimeUtc();
                    m.StartMonitor(limit);
                }
                try
                {
                    Util.SaveAsBuffer(wb, SaveFormat.Xlsx);
                    t = (DateTime.Now.ToFileTimeUtc() - t) / 10000;
                    Assert.Fail(msg + &quot;InterrupMonitor has not interrupted the process which finished in &quot; + t + &quot;ms&quot;);
                }
                catch (CellsException e)
                {
                    if (e.Code == ExceptionType.Interrupted)
                    {
                        t = (DateTime.Now.ToFileTimeUtc() - t) / 10000;
                        if (t &gt; (limit + limit + limit))
                        {
                            Assert.Fail(msg + &quot;InterrupMonitor took too long time, expected no more than 500 ms, but was &quot; + t + &quot;ms&quot;);
                        }
                        else
                        {
                            Console.WriteLine(msg + &quot;Interrupted after &quot; + t + &quot;ms&quot;);
                        }
                    }
                    else
                    {
                        throw e;
                    }
                }
            }
        }
```

### See Also

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


