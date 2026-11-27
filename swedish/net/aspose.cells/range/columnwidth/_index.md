---
title: "Range.ColumnWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Range-egenskap. Ställer in eller hämtar kolumnbredden för detta område"
type: docs
url: /sv/net/aspose.cells/range/columnwidth/
---
## Range.ColumnWidth property

Anger eller hämtar kolumnbredden för detta område

```csharp
public double ColumnWidth { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RangePropertyColumnWidthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Få åtkomst till ett område (kolumner B till D)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("B:D");
            
            // Visa aktuell kolumnbredd
            Console.WriteLine("Current ColumnWidth: " + range.ColumnWidth);

            // Ställ in ny kolumnbredd (i teckenenheter)
            range.ColumnWidth = 15.0;

            // Fyll i celler för att demonstrera effekten
            worksheet.Cells["B1"].PutValue("This is column B");
            worksheet.Cells["C1"].PutValue("This is column C");
            worksheet.Cells["D1"].PutValue("This is column D");

            // Anpassa rader automatiskt för att visa innehållet
            worksheet.AutoFitRows();

            // Spara arbetsboken
            workbook.Save("ColumnWidthDemo.xlsx");
        }
    }
}
```

### Se även

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


