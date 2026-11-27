---
title: "PivotField.IsInsertPageBreaksBetweenItems"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField egenskap. Anger om sidbrytningar ska infogas efter varje objekt. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/isinsertpagebreaksbetweenitems/
---
## PivotField.IsInsertPageBreaksBetweenItems property

Anger om sidbrytningar ska infogas efter varje objekt. Standardvärdet är false.

```csharp
public bool IsInsertPageBreaksBetweenItems { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsInsertPageBreaksBetweenItemsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 7; i++)
            {
                worksheet.Cells["A" + i].PutValue("Category " + (i % 3 + 1));
                worksheet.Cells["B" + i].PutValue(i * 100);
            }

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B7", "E3", "PivotTable");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Kontrollera sidantalet innan egenskapen sätts
            SheetRender render1 = new SheetRender(worksheet, new ImageOrPrintOptions());
            Console.WriteLine("Page count before: " + render1.PageCount);

            // Ställ in egenskapen IsInsertPageBreaksBetweenItems
            PivotField field = pivotTable.RowFields[0];
            field.IsInsertPageBreaksBetweenItems = true;
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Kontrollera sidantalet efter att egenskapen har satts
            SheetRender render2 = new SheetRender(worksheet, new ImageOrPrintOptions());
            Console.WriteLine("Page count after: " + render2.PageCount);

            // Spara arbetsboken
            workbook.Save("PivotFieldIsInsertPageBreaksBetweenItemsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


