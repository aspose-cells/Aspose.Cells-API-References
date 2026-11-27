---
title: "ProtectedRange.CellArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ProtectedRange-egenskap. Hämtar CellArea-objektet som representerar cellområdet som ska skyddas"
type: docs
url: /sv/net/aspose.cells/protectedrange/cellarea/
---
## ProtectedRange.CellArea property

Hämtar `CellArea`-objektet som representerar cellområdet som ska skyddas.

```csharp
public CellArea CellArea { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectedRangePropertyCellAreaDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa skyddade områden
            ProtectedRangeCollection allowRanges = worksheet.AllowEditRanges;
            
            // Lägg till första skyddade området
            int index1 = allowRanges.Add("Range1", 0, 0, 2, 2);
            ProtectedRange range1 = allowRanges[index1];
            range1.Password = "123";

            // Lägg till andra skyddade området
            int index2 = allowRanges.Add("Range2", 3, 3, 5, 5);
            ProtectedRange range2 = allowRanges[index2];
            range2.Password = "456";

            // Visa CellArea-information för båda områdena
            Console.WriteLine("Protected Range 1:");
            Console.WriteLine($"Name: {range1.Name}");
            Console.WriteLine($"Area: {range1.CellArea.StartRow},{range1.CellArea.StartColumn} to {range1.CellArea.EndRow},{range1.CellArea.EndColumn}");

            Console.WriteLine("\nProtected Range 2:");
            Console.WriteLine($"Name: {range2.Name}");
            Console.WriteLine($"Area: {range2.CellArea.StartRow},{range2.CellArea.StartColumn} to {range2.CellArea.EndRow},{range2.CellArea.EndColumn}");

            // Spara arbetsboken
            workbook.Save("ProtectedRangeDemo.xlsx");
        }
    }
}
```

### Se även

* struct [CellArea](../../cellarea/)
* class [ProtectedRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


