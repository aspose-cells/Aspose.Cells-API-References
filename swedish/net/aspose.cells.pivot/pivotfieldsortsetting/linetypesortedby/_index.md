---
title: "PivotFieldSortSetting.LineTypeSortedBy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotFieldSortSetting-egenskap. Pivotlinjetypen som sorteras efter"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfieldsortsetting/linetypesortedby/
---
## PivotFieldSortSetting.LineTypeSortedBy property

Pivotlinjetypen som sorteras efter.

```csharp
public PivotLineType LineTypeSortedBy { get; }
```

### Anmärkningar

Fungerar endast när detta fält inte sorteras efter etiketter.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldSortSettingPropertyLineTypeSortedByDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 5;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            
            // Sortera i stigande ordning med linjetyp – ange en tom sträng för cellName‑parametern
            pivotTable.RowFields[0].SortBy(SortOrder.Ascending, 0, PivotLineType.GrandTotal, "");
            
            // Demonstrera LineTypeSortedBy-egenskap
            Console.WriteLine("LineTypeSortedBy: " + pivotTable.RowFields[0].SortSetting.LineTypeSortedBy);
            
            // Ändra sortering för att använda vanlig radtyp
            pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "C5");
            Console.WriteLine("LineTypeSortedBy after change: " + pivotTable.RowFields[0].SortSetting.LineTypeSortedBy);
        }
    }
}
```

### Se även

* enum [PivotLineType](../../pivotlinetype/)
* class [PivotFieldSortSetting](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


