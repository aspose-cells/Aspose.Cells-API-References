---
title: "SystemTimeInterruptMonitor.StartMonitor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SystemTimeInterruptMonitor. Inicia el monitor con el límite de tiempo especificado. El tiempo de inicio para calcular el costo de tiempo es justo cuando se llama a este método, por lo que el procedimiento que necesita ser monitorizado debe iniciarse justo después de esta llamada."
type: docs
url: /es/net/aspose.cells/systemtimeinterruptmonitor/startmonitor/
---
## SystemTimeInterruptMonitor.StartMonitor method

Inicia el monitor con el límite de tiempo especificado. El tiempo de inicio para calcular el tiempo consumido es justo cuando se llama a este método, por lo que el procedimiento que necesita ser monitorizado debe iniciarse justo después de esta llamada.

```csharp
public void StartMonitor(int msLimit)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| msLimit | Int32 | límite de tiempo (ms) para requerir la interrupción. |

### Ejemplos

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

### Ver también

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


