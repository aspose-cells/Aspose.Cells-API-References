---
title: "Cell.Calculate"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Methode. Berechnet die Formel der Zelle"
type: docs
url: /de/net/aspose.cells/cell/calculate/
---
## Cell.Calculate method

Berechnet die Formel der Zelle.

```csharp
public void Calculate(CalculationOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Optionen | CalculationOptions | Optionen für die Berechnung |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodCalculateWithCalculationOptionsDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Setze eine einfache Formel in Zelle A1
            Cell cellA1 = worksheet.Cells["A1"];
            cellA1.Formula = "=SUM(1, 2, 3)";
            
            // Berechne mit den Standardoptionen
            cellA1.Calculate(new CalculationOptions());
            Console.WriteLine("A1 value after calculation: " + cellA1.Value);

            // Setze eine Array-Formel im Bereich B1:D1
            Cell cellB1 = worksheet.Cells["B1"];
            cellB1.SetArrayFormula("={1,2,3}", 1, 3);
            
            // Berechne die Array-Formel mit Optionen
            cellB1.Calculate(new CalculationOptions());
            Console.WriteLine("B1 value after calculation: " + cellB1.Value);

            // Setze eine komplexere Formel in Zelle A2
            Cell cellA2 = worksheet.Cells["A2"];
            cellA2.Formula = "=IF(A1>5, \"Greater\", \"Less or equal\")";
            
            // Berechne mit Optionen
            cellA2.Calculate(new CalculationOptions());
            Console.WriteLine("A2 value after calculation: " + cellA2.Value);
        }
    }
}
```

### Siehe auch

* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


