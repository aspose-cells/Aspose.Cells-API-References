---
title: "Workbook.InterruptMonitor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Workbook property. Ottiene e imposta il monitor di interruzione"
type: docs
url: /it/net/aspose.cells/workbook/interruptmonitor/
---
## Workbook.InterruptMonitor property

Ottiene e imposta il monitor di interruzione.

```csharp
public AbstractInterruptMonitor InterruptMonitor { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyInterruptMonitorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni dati al worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Crea e assegna il monitor di interruzione
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;
            
            try
            {
                Console.WriteLine("Starting save operation...");
                
                // Simula un'operazione a lunga durata interrompendola immediatamente
                monitor.Interrupt();
                
                // Prova a salvare - dovrebbe essere interrotta
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

### Vedi anche

* class [AbstractInterruptMonitor](../../abstractinterruptmonitor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


