---
title: "ProtectedRange.CellArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ProtectedRange-Eigenschaft. Gibt das CellArea-Objekt zurück, das den zu schützenden Zellbereich darstellt"
type: docs
url: /de/net/aspose.cells/protectedrange/cellarea/
---
## ProtectedRange.CellArea property

Gibt das `CellArea`-Objekt zurück, das den zu schützenden Zellbereich darstellt.

```csharp
public CellArea CellArea { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyCellAreaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle geschützte Bereiche
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;
            
            // Füge den ersten geschützten Bereich hinzu
            int index1 = allowRanges.Add("Range1", 0, 0, 2, 2);
            ProtectedRange range1 = allowRanges[index1];
            range1.Password = "123";

            // Füge den zweiten geschützten Bereich hinzu
            int index2 = allowRanges.Add("Range2", 3, 3, 5, 5);
            ProtectedRange range2 = allowRanges[index2];
            range2.Password = "456";

            // Zeige CellArea-Informationen für beide Bereiche an
            Console.WriteLine("Protected Range 1:");
            Console.WriteLine($"Name: {range1.Name}");
            Console.WriteLine($"Area: {range1.CellArea.StartRow},{range1.CellArea.StartColumn} to {range1.CellArea.EndRow},{range1.CellArea.EndColumn}");

            Console.WriteLine("\nProtected Range 2:");
            Console.WriteLine($"Name: {range2.Name}");
            Console.WriteLine($"Area: {range2.CellArea.StartRow},{range2.CellArea.StartColumn} to {range2.CellArea.EndRow},{range2.CellArea.EndColumn}");

            // Speichere die Arbeitsmappe
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


