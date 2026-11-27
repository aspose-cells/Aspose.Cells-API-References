---
title: "PivotField.ShowAllItems"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField‑egenskap. Anger om alla objekt ska visas i PivotTable‑vyn även om de inte innehåller sammanfattningsdata. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/showallitems/
---
## PivotField.ShowAllItems property

Anger om alla objekt ska visas i PivotTable-vyn, även om de inte innehåller sammanfattningsdata. Standardvärdet är falskt.

```csharp
public bool ShowAllItems { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowAllItemsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Exempeldatat för pivottabell
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Product");
            sheet.Cells["C1"].PutValue("Sales");
            
            sheet.Cells["A2"].PutValue("Electronics");
            sheet.Cells["B2"].PutValue("Laptop");
            sheet.Cells["C2"].PutValue(1200);
            
            sheet.Cells["A3"].PutValue("Electronics");
            sheet.Cells["B3"].PutValue("Phone");
            sheet.Cells["C3"].PutValue(800);
            
            sheet.Cells["A4"].PutValue("Furniture");
            sheet.Cells["B4"].PutValue("Chair");
            sheet.Cells["C4"].PutValue(150);

            // Lägg till pivottabell
            int index = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");

            // Ställ in ShowAllItems‑egenskapen för radfältet
            PivotField rowField = pivotTable.RowFields[0];
            rowField.ShowAllItems = true;

            // Beräkna data och spara
            pivotTable.CalculateData();
            workbook.Save("PivotFieldShowAllItemsDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


