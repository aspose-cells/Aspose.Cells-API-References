---
title: "Klass PivotTableFormat"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Pivot.PivotTableFormat-klass. Representerar formatet som definieras i pivottabellen"
type: docs
url: /sv/net/aspose.cells.pivot/pivottableformat/
---
## PivotTableFormat class

Representerar formatet som definierats i PivotTable.

```csharp
public class PivotTableFormat
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [PivotArea](../../aspose.cells.pivot/pivottableformat/pivotarea/) { get; } | Hämtar pivotområdet. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| [GetStyle](../../aspose.cells.pivot/pivottableformat/getstyle/)() | Hämtar den formaterade stilen. |
| [SetStyle](../../aspose.cells.pivot/pivottableformat/setstyle/)(Style) | Ställer in stilen för pivotområdet. |

### Exempel

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotTableFormatDemo
    {
        public static void RunDemo()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);

            // Lägg till en pivottabell
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Lägg till fält i pivottabellen
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Kom åt PivotTableFormatCollection
            PivotTableFormatCollection pivotFormats = pivotTable.PivotFormats;

            // Lägg till ett nytt format i samlingen
            int formatIndex = pivotFormats.Add();
            PivotTableFormat pivotFormat = pivotFormats[formatIndex];

            // Åtkomst till PivotArea för formatet
            PivotArea pivotArea = pivotFormat.PivotArea;
            pivotArea.AxisType = PivotFieldType.Data;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;

            // Skapa en ny stil
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Applicera stilen på PivotTableFormat
            pivotFormat.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("PivotTableFormatDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


