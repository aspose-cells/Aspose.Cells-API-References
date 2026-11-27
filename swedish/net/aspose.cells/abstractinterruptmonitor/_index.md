---
title: "Klass AbstractInterruptMonitor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.AbstractInterruptMonitor-klass. Övervakar avbrottsförfrågningar i alla tidskrävande operationer"
type: docs
url: /sv/net/aspose.cells/abstractinterruptmonitor/
---
## AbstractInterruptMonitor class

Övervaka avbrottsförfrågningar i alla tidskrävande operationer.

```csharp
public abstract class AbstractInterruptMonitor
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| abstract [IsInterruptionRequested](../../aspose.cells/abstractinterruptmonitor/isinterruptionrequested/) { get; } | Anger om avbrott begärs för den aktuella operationen. Om sant kommer den aktuella operationen att avbrytas. Implementeringen bör utföra en snabb och effektiv kontroll här, annars kan den bli en flaskhals för proceduren. |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | När proceduren avbryts, om proceduren ska avslutas tyst eller kasta ett Exception. Standard är falskt, det vill säga, när [`IsInterruptionRequested`](./isinterruptionrequested/) är true, kommer ett [`CellsException`](../cellsexception/) med kod Interrupted att kastas. |

### Exempel

```csharp
using Aspose.Cells;
using System;
using System.Reflection.Metadata.Ecma335;

namespace AsposeCellsExamples
{
    // Anpassad implementation av AbstractInterruptMonitor
    public class CustomInterruptMonitor : AbstractInterruptMonitor
    {
        //resultatfilen är korrekt
        public override bool IsInterruptionRequested
        {
            get
            {
                Console.WriteLine("Get the return value of whether to interrupt the program===");
                // Logik för att avgöra om avbrott begärs
                return false; // Change this based on your logic
            }
        }

        public override bool TerminateWithoutException
        {
            get => false; // Change this based on your logic
        }

        //// resultatfilen kraschar
        //public override bool IsInterruptionRequested
        //{
        //    get
        //    {
        //        Console.WriteLine("Hämta returvärdet för om programmet ska avbrytas===");
        //        // Logik för att avgöra om avbrott begärs
        //        //return false; // Ändra detta baserat på din logik
        //        return true;
        //    }
        //}

        //public override bool TerminateWithoutException
        //{
        //    get => true; // Ändra detta baserat på din logik
        //}
    }

    public class InterruptMonitorDemo
    {
        public static void RunDemo()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].Formula = "=A1+A2";

            // Skapa en instans av CustomInterruptMonitor
            CustomInterruptMonitor monitor = new CustomInterruptMonitor();

            // Ställ in laddningsalternativ med den anpassade avbrottsövervakaren
            LoadOptions loadOptions = new LoadOptions
            {
                InterruptMonitor = monitor
            };

            // Läs in arbetsboken med de angivna alternativen
            workbook = new Workbook("Sample.xlsx", loadOptions);

            // Utför beräkningar
            workbook.CalculateFormula();

            // Spara arbetsboken
            workbook.Save("InterruptMonitorDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


