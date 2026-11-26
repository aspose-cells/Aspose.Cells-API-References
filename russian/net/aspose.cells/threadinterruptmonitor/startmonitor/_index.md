---
title: "ThreadInterruptMonitor.StartMonitor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ThreadInterruptMonitor. Запускает монитор с указанным временным ограничением. Время начала для расчёта затраченного времени берётся в момент вызова этого метода, поэтому процедура, которую нужно мониторить, должна быть запущена сразу после этого вызова."
type: docs
url: /ru/net/aspose.cells/threadinterruptmonitor/startmonitor/
---
## ThreadInterruptMonitor.StartMonitor method

Запускает монитор с указанным ограничением времени. Время начала для расчёта затраченного времени устанавливается в момент вызова этого метода, поэтому процедура, которую необходимо мониторить, должна быть запущена сразу после этого вызова.

```csharp
public void StartMonitor(int msLimit)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| msLimit | Int32 | ограничение времени (мс), при котором требуется прерывание. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodStartMonitorWithInt32Demo
    {
        public static void Run()
        {
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            monitor.StartMonitor(1000);

            try
            {
                Workbook wb = new Workbook("Large.xlsx", lopts);
                monitor.FinishMonitor();

                monitor.StartMonitor(1500);
                wb.Save("result.xlsx");
                monitor.FinishMonitor();
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception: " + ex.Message);
            }
        }
    }
}
```

### См. также

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


