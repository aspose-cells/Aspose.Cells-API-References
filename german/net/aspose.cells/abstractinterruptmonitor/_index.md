---
title: "Klasse AbstractInterruptMonitor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.AbstractInterruptMonitor Klasse. Überwacht Unterbrechungsanfragen bei allen zeitaufwändigen Vorgängen"
type: docs
url: /de/net/aspose.cells/abstractinterruptmonitor/
---
## AbstractInterruptMonitor class

Überwacht Unterbrechungsanfragen bei allen zeitintensiven Vorgängen.

```csharp
public abstract class AbstractInterruptMonitor
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| abstract [IsInterruptionRequested](../../aspose.cells/abstractinterruptmonitor/isinterruptionrequested/) { get; } | Gibt an, ob für den aktuellen Vorgang eine Unterbrechung angefordert wird. Wenn true, wird der aktuelle Vorgang unterbrochen. Die Implementierung sollte hier eine schnelle und effiziente Prüfung durchführen, sonst könnte sie zum weiteren Engpass für den Vorgang werden. |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | Wenn der Vorgang unterbrochen wird, ob er stillschweigend beendet oder eine Exception ausgelöst wird. Standard ist false, das heißt, wenn [`IsInterruptionRequested`](./isinterruptionrequested/) true ist, wird eine [`CellsException`](../cellsexception/) mit dem Code Interrupted ausgelöst. |

### Beispiele

```csharp
using Aspose.Cells;
using System;
using System.Reflection.Metadata.Ecma335;

namespace AsposeCellsExamples
{
    // Benutzerdefinierte Implementierung von AbstractInterruptMonitor
    public class CustomInterruptMonitor : AbstractInterruptMonitor
    {
        //Die Ergebnisdatei ist korrekt
        public override bool IsInterruptionRequested
        {
            get
            {
                Console.WriteLine("Get the return value of whether to interrupt the program===");
                // Logik zur Bestimmung, ob eine Unterbrechung angefordert wird
                return false; // Change this based on your logic
            }
        }

        public override bool TerminateWithoutException
        {
            get => false; // Change this based on your logic
        }

        //// die Ergebnisdatei stürzt ab
        //public override bool IsInterruptionRequested
        //{
        //    get
        //    {
        //        Console.WriteLine("Get the return value of whether to interrupt the program===");
        //        // Logik zur Bestimmung, ob eine Unterbrechung angefordert wird
        //        //return false; // Ändern Sie dies basierend auf Ihrer Logik
        //        return true;
        //    }
        //}

        //public override bool TerminateWithoutException
        //{
        //    get => true; // Ändern Sie dies basierend auf Ihrer Logik
        //}
    }

    public class InterruptMonitorDemo
    {
        public static void RunDemo()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].Formula = "=A1+A2";

            // Erstellen Sie eine Instanz von CustomInterruptMonitor
            CustomInterruptMonitor monitor = new CustomInterruptMonitor();

            // Setzen Sie Ladeoptionen mit dem benutzerdefinierten CustomInterruptMonitor
            LoadOptions loadOptions = new LoadOptions
            {
                InterruptMonitor = monitor
            };

            // Laden Sie die Arbeitsmappe mit den angegebenen Optionen
            workbook = new Workbook("Sample.xlsx", loadOptions);

            // Führen Sie Berechnungen durch
            workbook.CalculateFormula();

            // Speichere die Arbeitsmappe
            workbook.Save("InterruptMonitorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


