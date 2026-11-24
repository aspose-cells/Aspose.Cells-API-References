---
title: "Worksheet.Cells"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Eigenschaft. Gibt die Cells-Sammlung zurück"
type: docs
url: /de/net/aspose.cells/worksheet/cells/
---
## Worksheet.Cells property

Gibt die [`Cells`](../../cells/) Sammlung zurück.

```csharp
public Cells Cells { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCellsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Auf die Cells-Sammlung zugreifen
            Cells cells = worksheet.Cells;
            
            // Werte in Cells setzen
            cells["A1"].PutValue("Item");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Apple");
            cells["B2"].PutValue(2.5);
            cells["A3"].PutValue("Orange");
            cells["B3"].PutValue(1.8);
            
            // Formel festlegen, um die Summe zu berechnen
            cells["A4"].PutValue("Total:");
            cells["B4"].Formula = "=SUM(B2:B3)";
            
            // Formeln berechnen
            workbook.CalculateFormula();
            
            // Zellwerte anzeigen
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("B1: " + cells["B1"].StringValue);
            Console.WriteLine("A2: " + cells["A2"].StringValue);
            Console.WriteLine("B2: " + cells["B2"].StringValue);
            Console.WriteLine("A3: " + cells["A3"].StringValue);
            Console.WriteLine("B3: " + cells["B3"].StringValue);
            Console.WriteLine("A4: " + cells["A4"].StringValue);
            Console.WriteLine("B4: " + cells["B4"].StringValue + " (Formula: " + cells["B4"].Formula + ")");
            
            // Arbeitsmappe speichern.
            workbook.Save("CellsPropertyDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [Cells](../../cells/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


