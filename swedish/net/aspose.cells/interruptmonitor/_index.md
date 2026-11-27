---
title: "Klass InterruptMonitor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.InterruptMonitor klass. Representerar alla operatörer för avbrottet."
type: docs
url: /sv/net/aspose.cells/interruptmonitor/
---
## InterruptMonitor class

Representerar alla operatörer för avbrottet.

```csharp
public class InterruptMonitor : AbstractInterruptMonitor
```

## Konstruktörer

| Namn | Beskrivning |
| --- | --- |
| [InterruptMonitor](interruptmonitor/)() | Standardkonstruktorn. |

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/interruptmonitor/isinterruptionrequested/) { get; } | Markera övervakaren som begär avbrott |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | När proceduren avbryts, om den ska avslutas tyst eller kasta ett undantag. Standard är falskt, det vill säga, när [`IsInterruptionRequested`](../abstractinterruptmonitor/isinterruptionrequested/) är sant, kastas ett [`CellsException`](../cellsexception/) med koden Interrupted. (Ärvd från [`AbstractInterruptMonitor`](../abstractinterruptmonitor/).) |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [Interrupt](../../aspose.cells/interruptmonitor/interrupt/)() | Avbryt den aktuella operatören. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassInterruptMonitorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till lite exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Skapa och tilldela avbrottsövervakare
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;
            
            try
            {
                Console.WriteLine("Starting save operation...");
                
                // Simulera avbrott av operationen
                monitor.Interrupt();
                
                // Försök att spara (bör avbrytas)
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
                    Console.WriteLine("Error occurred: " + e.Message);
                }
            }
        }
    }
}
```

### Se även

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


