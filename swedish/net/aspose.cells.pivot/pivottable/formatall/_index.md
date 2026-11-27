---
title: "PivotTable.FormatAll"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Formatera alla celler i pivottabellområdet"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/formatall/
---
## PivotTable.FormatAll method

Formatera alla celler i pivottabellområdet

```csharp
public void FormatAll(Style style)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| style | Stil | Stil som ska formateras |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFormatAllWithStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            var cells = worksheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 5;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 7;
            
            // Skapa pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int pivotIndex = pivotTables.Add("=Sheet1!A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[pivotIndex];
            
            // Lägg till fält i pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Skapa och konfigurera stil
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 10;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            style.Pattern = BackgroundType.Solid;
            
            // Tillämpa stil på hela pivottabellen
            pivotTable.FormatAll(style);
            
            // Spara arbetsboken
            workbook.Save("PivotTableFormatAllDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


