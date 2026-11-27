---
title: "PivotArea.IsRowGrandIncluded"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotArea-egenskap. Anger om radens totalsumma är inkluderad"
type: docs
url: /sv/net/aspose.cells.pivot/pivotarea/isrowgrandincluded/
---
## PivotArea.IsRowGrandIncluded property

Anger om radens totalsumma är inkluderad.

```csharp
public bool IsRowGrandIncluded { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyIsRowGrandIncludedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Exempeldata
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);

            // Skapa pivottabell
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Lägg till fält
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Skapa pivotformat
            int formatIndex = pivotTable.PivotFormats.Add();
            PivotTableFormat pivotFormat = pivotTable.PivotFormats[formatIndex];
            PivotArea pivotArea = pivotFormat.PivotArea;
            
            // Demonstrera IsRowGrandIncluded-egenskapen
            pivotArea.AxisType = PivotFieldType.Data;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = false;

            // Tillämpa stil för att markera totalraden
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGreen;
            style.Pattern = BackgroundType.Solid;
            pivotFormat.SetStyle(style);

            workbook.Save("PivotAreaIsRowGrandIncludedDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


