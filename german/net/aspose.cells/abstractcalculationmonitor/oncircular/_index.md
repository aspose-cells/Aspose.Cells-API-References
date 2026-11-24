---
title: "AbstractCalculationMonitor.OnCircular"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AbstractCalculationMonitor method. Implementieren Sie diese Methode, um Geschäftslogik auszuführen, wenn Formeln mit zirkulären Verweisen berechnet werden"
type: docs
url: /de/net/aspose.cells/abstractcalculationmonitor/oncircular/
---
## AbstractCalculationMonitor.OnCircular method

Implementieren Sie diese Methode, um Geschäftslogik auszuführen, wenn Formeln mit zirkulären Verweisen berechnet werden.

```csharp
public virtual bool OnCircular(IEnumerator circularCellsData)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| circularCellsData | IEnumerator | IEnumerator mit [`CalculationCell`](../../calculationcell/) Elementen, die Zellen darstellen, die von zirkulären Verweisen abhängen. |

### Rückgabewert

Ob die Formelmotor nach diesem Aufruf diese Zellen zirkulär berechnen muss. Wahr, um dem Formelmotor zu erlauben, die Berechnung für sie fortzusetzen. Falsch, um den Formelmotor nur diese Zellen als Berechnet zu markieren.

### Hinweise

In der Implementierung kann der Benutzer auch den erwarteten Wert als berechnetes Ergebnis für einen Teil/alle diese Zellen festlegen, sodass der Formelmotor sie nicht rekursiv berechnet.

### Beispiele

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

            // Ein Szenario für zirkuläre Verweise erstellen
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

### Siehe auch

* class [AbstractCalculationMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


