---
title: "SystemTimeInterruptMonitor.StartMonitor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод SystemTimeInterruptMonitor. Запускает монитор с указанным ограничением времени. Время начала для расчёта затраченного времени берётся в момент вызова этого метода, поэтому процедура, которую необходимо мониторить, должна быть запущена сразу после этого вызова."
type: docs
url: /ru/net/aspose.cells/systemtimeinterruptmonitor/startmonitor/
---
## SystemTimeInterruptMonitor.StartMonitor method

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
    public class SystemTimeInterruptMonitorMethodStartMonitorWithInt32Demo
    {
        public static void Run()
        {
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            monitor.StartMonitor(1000); // 1 second time limit

            try
            {
                Workbook wb = new Workbook("Large.xlsx", lopts);
                monitor.StartMonitor(1500); // 1.5 second time limit
                wb.Save("SystemTimeInterruptMonitorExample.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Operation interrupted: " + ex.Message);
            }
        }
    }
}
```

### См. также

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


