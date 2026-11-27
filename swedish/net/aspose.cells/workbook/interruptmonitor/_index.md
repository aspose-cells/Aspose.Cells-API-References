---
title: "Workbook.InterruptMonitor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-egenskap. Hämtar och sätter avbrottsövervakaren"
type: docs
url: /sv/net/aspose.cells/workbook/interruptmonitor/
---
## Workbook.InterruptMonitor property

Hämtar och anger avbrottsövervakaren.

```csharp
public AbstractInterruptMonitor InterruptMonitor { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyInterruptMonitorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till lite data i kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Skapa och tilldela avbrottsövervakare
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;
            
            try
            {
                Console.WriteLine("Starting save operation...");
                
                // Simulera en långvarig operation genom att avbryta omedelbart
                monitor.Interrupt();
                
                // Försök att spara - bör avbrytas
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

### Se även

* class [AbstractInterruptMonitor](../../abstractinterruptmonitor/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


