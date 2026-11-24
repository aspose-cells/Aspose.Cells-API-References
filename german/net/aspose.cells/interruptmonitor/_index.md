---
title: "Klasse InterruptMonitor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.InterruptMonitor Klasse. Stellt alle Vorgänge im Zusammenhang mit dem Abbruch dar"
type: docs
url: /de/net/aspose.cells/interruptmonitor/
---
## InterruptMonitor class

Stellt alle Operatoren zum Interrupt dar.

```csharp
public class InterruptMonitor : AbstractInterruptMonitor
```

## Konstruktoren

| Name | Beschreibung |
| --- | --- |
| [InterruptMonitor](interruptmonitor/)() | Der Standardkonstruktor. |

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/interruptmonitor/isinterruptionrequested/) { get; } | Den Monitor als Unterbrechungsanforderung markieren |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | Wenn das Verfahren unterbrochen wird, ob das Verfahren stillschweigend beendet oder eine Ausnahme ausgelöst wird. Standard ist false, das heißt, wenn [`IsInterruptionRequested`](../abstractinterruptmonitor/isinterruptionrequested/) true ist, wird eine [`CellsException`](../cellsexception/) mit dem Code Interrupted ausgelöst. (Geerbt von [`AbstractInterruptMonitor`](../abstractinterruptmonitor/).) |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Interrupt](../../aspose.cells/interruptmonitor/interrupt/)() | Den aktuellen Vorgang unterbrechen. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassInterruptMonitorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Fügen Sie einige Beispieldaten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // InterruptMonitor erstellen und zuweisen
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;
            
            try
            {
                Console.WriteLine("Starting save operation...");
                
                // Unterbrechung des Vorgangs simulieren
                monitor.Interrupt();
                
                // Versuch zu speichern (sollte unterbrochen werden)
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

### Siehe auch

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


