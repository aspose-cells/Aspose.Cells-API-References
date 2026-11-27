---
title: "PivotTable.FormatRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Formatera raddata i pivottabellområdet"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/formatrow/
---
## PivotTable.FormatRow method

Formatera raddata i pivottabellområdet

```csharp
public void FormatRow(int row, Style style)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Int32 | Radindex för Row-objektet |
| style | Stil | Stil som ska formateras |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodFormatRowWithInt32StyleDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook wb = new Workbook();
            Worksheet worksheet = wb.Worksheets[0];
            
            // Exempeldatat för pivottabell
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // Skapa pivottabell
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Skapa stil för formatering
            Style style = wb.CreateStyle();
            style.Custom = "0.00%";
            style.Font.Name = "Calibri";
            style.Font.Size = 11;
            
            // Hitta och formatera rader
            Cell cell = worksheet.Cells.Find("A", null);
            if (cell != null)
            {
                pivotTable.FormatRow(cell.Row, style);
            }
            
            cell = worksheet.Cells.Find("B", null);
            if (cell != null)
            {
                pivotTable.FormatRow(cell.Row, style);
            }
            
            // Spara arbetsboken
            wb.Save("PivotTableFormatRowDemo.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../../aspose.cells/style/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


