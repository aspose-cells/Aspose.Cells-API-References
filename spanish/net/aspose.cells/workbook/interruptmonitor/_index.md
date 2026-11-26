---
title: "Workbook.InterruptMonitor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Workbook. Obtiene y establece el monitor de interrupción"
type: docs
url: /es/net/aspose.cells/workbook/interruptmonitor/
---
## Workbook.InterruptMonitor property

Obtiene y establece el monitor de interrupción.

```csharp
public AbstractInterruptMonitor InterruptMonitor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyInterruptMonitorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunos datos a la hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Crea y asigna el monitor de interrupción
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;
            
            try
            {
                Console.WriteLine("Starting save operation...");
                
                // Simular una operación de larga duración interrumpiéndola inmediatamente
                monitor.Interrupt();
                
                // Intentar guardar - debería ser interrumpido
                workbook.Save("output.pdf", SaveFormat.Pdf);
                Console.WriteLine("Save completed successfully.");
            }
            catch (CellsException e)
            {
                if (e.Code == ExceptionType.Interrupted)
                {
                    Console.WriteLine("Operation was successfully interrupted.");
                }
                else
                {
                    Console.WriteLine($"Error occurred: {e.Message}");
                }
            }
        }
    }
}
```

### Ver también

* class [AbstractInterruptMonitor](../../abstractinterruptmonitor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


