---
title: "InterruptMonitor.Interrupt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método InterruptMonitor. Interrumpe al operador actual"
type: docs
url: /es/net/aspose.cells/interruptmonitor/interrupt/
---
## InterruptMonitor.Interrupt method

Interrumpe el operador actual.

```csharp
public void Interrupt()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class InterruptMonitorMethodInterruptDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunos datos a la hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 10000; i++)
            {
                worksheet.Cells[i, 0].Value = "Data " + i;
            }

            // Crear y establecer el monitor de interrupción
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            try
            {
                Console.WriteLine("Starting long operation...");
                
                // Simular una operación larga en otro hilo
                System.Threading.ThreadPool.QueueUserWorkItem(_ => 
                {
                    System.Threading.Thread.Sleep(1000); // Wait 1 second
                    Console.WriteLine("Interrupting operation...");
                    monitor.Interrupt(); // Call interrupt
                });

                // Ejecutar una operación larga (guardar)
                workbook.Save("output.pdf", SaveFormat.Pdf);
                Console.WriteLine("Operation completed successfully.");
            }
            catch (CellsException e)
            {
                if (e.Code == ExceptionType.Interrupted)
                {
                    Console.WriteLine("Operation was interrupted successfully.");
                }
                else
                {
                    Console.WriteLine("Error: " + e.Message);
                }
            }
        }
    }
}
```

### Ver también

* class [InterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


