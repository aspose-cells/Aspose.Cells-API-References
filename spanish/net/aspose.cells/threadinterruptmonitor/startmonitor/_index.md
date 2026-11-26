---
title: "ThreadInterruptMonitor.StartMonitor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ThreadInterruptMonitor. Inicia el monitor con el límite de tiempo especificado. El tiempo de inicio para calcular el tiempo transcurrido es justo cuando se llama a este método, por lo que el procedimiento que necesita ser monitorizado debe iniciarse justo después de esta llamada"
type: docs
url: /es/net/aspose.cells/threadinterruptmonitor/startmonitor/
---
## ThreadInterruptMonitor.StartMonitor method

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

### Ver también

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


