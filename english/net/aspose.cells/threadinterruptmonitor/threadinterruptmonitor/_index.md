---
title: ThreadInterruptMonitor.ThreadInterruptMonitor
second_title: Aspose.Cells for .NET API Reference
description: ThreadInterruptMonitor constructor. Constructs one interruption monitor
type: docs
url: /net/aspose.cells/threadinterruptmonitor/threadinterruptmonitor/
---
## ThreadInterruptMonitor constructor

Constructs one interruption monitor.

```csharp
public ThreadInterruptMonitor(bool terminateWithoutException)
```

| Parameter | Type | Description |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |

### Examples

```csharp
// Called: ThreadInterruptMonitor m = new ThreadInterruptMonitor(false);
[Test]
        public void ThreadInterruptMonitor_Constructor()
        {
            for (int i = 0; i < 2; i++)
            {
                long t = DateTime.Now.ToFileTimeUtc();
                Workbook wb = new Workbook();
                Model.RandomFill(wb.Worksheets[0].Cells, 5000, 20, true);
                int limit = ((int)((DateTime.Now.ToFileTimeUtc() - t) / 10000)) >> 2; //by test the time cost of saving is about half of that of filling
                string msg;
                if (i != 0)
                {
                    msg = "SystemTimeInterruptMonitor: ";
                    SystemTimeInterruptMonitor m = new SystemTimeInterruptMonitor(false);
                    wb.InterruptMonitor = m;
                    t = DateTime.Now.ToFileTimeUtc();
                    m.StartMonitor(limit);
                }
                else
                {
                    msg = "ThreadInterruptMonitor: ";
                    ThreadInterruptMonitor m = new ThreadInterruptMonitor(false);
                    wb.InterruptMonitor = m;
                    t = DateTime.Now.ToFileTimeUtc();
                    m.StartMonitor(limit);
                }
                try
                {
                    Util.SaveAsBuffer(wb, SaveFormat.Xlsx);
                    t = (DateTime.Now.ToFileTimeUtc() - t) / 10000;
                    Assert.Fail(msg + "InterrupMonitor has not interrupted the process which finished in " + t + "ms");
                }
                catch (CellsException e)
                {
                    if (e.Code == ExceptionType.Interrupted)
                    {
                        t = (DateTime.Now.ToFileTimeUtc() - t) / 10000;
                        if (t > (limit + limit + limit))
                        {
                            Assert.Fail(msg + "InterrupMonitor took too long time, expected no more than 500 ms, but was " + t + "ms");
                        }
                        else
                        {
                            Console.WriteLine(msg + "Interrupted after " + t + "ms");
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


