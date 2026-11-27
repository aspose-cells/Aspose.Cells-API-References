---
title: "PivotTable.PivotFormats"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Hämtar alla cellformat som tillämpas på denna pivottabell"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/pivotformats/
---
## PivotTable.PivotFormats property

Hämtar alla cellformat som tillämpas på denna pivottabell.

```csharp
public PivotTableFormatCollection PivotFormats { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPivotFormatsDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            sheet.Cells["A1"].Value = "Fruit";
            sheet.Cells["B1"].Value = "Quantity";
            sheet.Cells["A2"].Value = "Apple";
            sheet.Cells["B2"].Value = 10;
            sheet.Cells["A3"].Value = "Orange";
            sheet.Cells["B3"].Value = 15;
            sheet.Cells["A4"].Value = "Banana";
            sheet.Cells["B4"].Value = 20;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Skapa stil för formatering
            Style style = workbook.CreateStyle();
            style.BackgroundColor = System.Drawing.Color.LightBlue;
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, System.Drawing.Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, System.Drawing.Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, System.Drawing.Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, System.Drawing.Color.Black);

            // Applicera formatering på pivottabellens dataområde
            pivotTable.PivotFormats.FormatArea(
                PivotFieldType.Data, 
                0, 
                PivotFieldSubtotalType.None, 
                PivotTableSelectionType.DataAndLabel, 
                false, 
                false, 
                style);

            // Spara arbetsboken
            workbook.Save("PivotTableWithFormats.xlsx");
        }
    }
}
```

### Se även

* class [PivotTableFormatCollection](../../pivottableformatcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


