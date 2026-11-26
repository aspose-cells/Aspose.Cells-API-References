---
title: "ThreadInterruptMonitor.ThreadInterruptMonitor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor ThreadInterruptMonitor. Construye un monitor de interrupción"
type: docs
url: /es/net/aspose.cells/threadinterruptmonitor/threadinterruptmonitor/
---
## ThreadInterruptMonitor constructor

Construye un monitor de interrupción.

```csharp
public ThreadInterruptMonitor(bool terminateWithoutException)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Crear un ThreadInterruptMonitor con throwOnInterrupted configurado a false
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            workbook.InterruptMonitor = monitor;
            
            // Establecer un límite de tiempo corto (100 ms) para la demostración
            int timeLimit = 100;
            monitor.StartMonitor(timeLimit);

            try
            {
                // Ejecutar una operación larga (será interrumpida)
                for (int i = 0; i < 100000; i++)
                {
                    workbook.Worksheets[0].Cells[i % 100, i / 100].PutValue(i);
                }
                
                Console.WriteLine("Operation completed without interruption");
            }
            catch (CellsException e)
            {
                if (e.Code == ExceptionType.Interrupted)
                {
                    Console.WriteLine("Operation was successfully interrupted");
                }
                else
                {
                    Console.WriteLine("Error occurred: " + e.Message);
                }
            }
        }
    }
}
```

### Ver también

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


