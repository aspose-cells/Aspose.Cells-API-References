---
title: "AbstractCalculationMonitor.OnCircular"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AbstractCalculationMonitor-metod. Implementera den här metoden för att utföra affärslogik när du beräknar formler med cirkulära referenser"
type: docs
url: /sv/net/aspose.cells/abstractcalculationmonitor/oncircular/
---
## AbstractCalculationMonitor.OnCircular method

Implementera den här metoden för att utföra affärslogik när du beräknar formler med cirkulära referenser.

```csharp
public virtual bool OnCircular(IEnumerator circularCellsData)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| circularCellsData | IEnumerator | IEnumerator med [`CalculationCell`](../../calculationcell/) objekt som representerar celler som beror på cirkulära referenser. |

### Returvärde

Om formelmotorn behöver beräkna dessa celler i cirkulär ordning efter detta anrop. True för att låta formelmotorn fortsätta beräkna dem. False för att låta formelmotorn bara markera dessa celler som Calculated.

### Anmärkningar

I implementationen kan användaren även ange det förväntade värdet som beräknat resultat för del/alla av dessa celler så att formelmotorn inte beräknar dem rekursivt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Collections;

    public class AbstractCalculationMonitorMethodOnCircularDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa ett scenario med cirkulär referens
            worksheet.Cells["A1"].Formula = "=B1";
            worksheet.Cells["B1"].Formula = "=A1";

            CalculationOptions options = new CalculationOptions();
            options.CalculationMonitor = new CircularReferenceMonitor();

            try
            {
                workbook.CalculateFormula(options);
                Console.WriteLine("Calculation completed. Check console for circular reference handling.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Calculation error: {ex.Message}");
            }

            workbook.Save("OnCircularDemo.xlsx");
        }

        private class CircularReferenceMonitor : AbstractCalculationMonitor
        {
            public override bool OnCircular(IEnumerator circularCellsData)
            {
                Console.WriteLine("Circular reference detected!");
                while (circularCellsData.MoveNext())
                {
                    Console.WriteLine($"Circular cell: {circularCellsData.Current}");
                }
                return true; // Continue calculation
            }
        }
    }
}
```

### Se även

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


