---
title: "CalculationOptions.CalcStackSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "CalculationOptions-Eigenschaft. Die Stapelgröße für die rekursive Berechnung von Zellen. Der Standardwert ist 200"
type: docs
url: /de/net/aspose.cells/calculationoptions/calcstacksize/
---
## CalculationOptions.CalcStackSize property

Die Stapelgröße für die rekursive Berechnung von Zellen. Der Standardwert ist 200.

```csharp
public int CalcStackSize { get; set; }
```

### Hinweise

Wenn eine große Anzahl von Zellen rekursiv im Abhängigkeitsbaum berechnet werden muss, kann im Berechnungsprozess eine StackOverflowException auftreten. In diesem Fall sollte der Benutzer für diese Eigenschaft einen kleineren Wert angeben. Für solche Situationen muss der Benutzer den geeigneten Wert für diese Eigenschaft anhand der tatsächlichen Formeln und Daten bestimmen. Ein zu kleiner Wert kann jedoch die Leistungsfähigkeit der Formelberechnung beeinträchtigen, und ein Wert kleiner als 2 macht es unmöglich, eine Formel zu berechnen, die von einer anderen abhängt. Daher wird ein angegebener Wert, der kleiner als 2 ist, auf 2 zurückgesetzt.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationOptionsPropertyCalcStackSizeDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Richten Sie Beispiel-Formeln ein, die eine Stapelberechnung erfordern
            cells["A1"].PutValue(1);
            int last = 100;
            cells["B1"].Formula = "=SUM(A1:A" + last + ")";
            
            for (int i = 2; i <= last; i++)
            {
                cells["A" + i].Formula = "=A" + (i - 1) + "*1.1";
                cells["B" + i].Formula = "=B" + (i - 1) + "+A" + i;
            }

            // Berechnen mit benutzerdefinierter Stapelgröße
            wb.CalculateFormula(new CalculationOptions() { CalcStackSize = 50 });
            
            Console.WriteLine("Calculation completed with custom stack size");
        }
    }
}
```

### Siehe auch

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


