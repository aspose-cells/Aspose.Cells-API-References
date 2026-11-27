---
title: "PivotField.AutoShowField"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Representerar index för automatisk visning av fält. 1 betyder PivotField själv. Det bör vara indexet för datafälten"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/autoshowfield/
---
## PivotField.AutoShowField property

Representerar index för automatisk visning av fält. -1 betyder PivotField själv. Det bör vara indexet för datafälten.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.RankBy property or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AutoShowField { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotField.Top10AutoShowSettings.RankBy eller metoden PivotField.Top10AutoShow(). Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyAutoShowFieldDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad och fyll i med exempeldata
            Worksheet sheet = workbook.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Lägg till exempeldata för pivottabell
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 20;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 15;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 5;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 10;
            
            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Lägg till radfält och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Konfigurera AutoShow för det första pivottfältet
            PivotField pivotField = pivotTable.RowFields[0];
            pivotField.AutoShowCount = 2;
            pivotField.AutoShowField = 1; // Index of data field (Quantity)
            pivotField.IsAutoShow = true;
            pivotField.IsAscendShow = true; // Equivalent to "Top" in AutoShowType
            
            // Spara arbetsboken
            workbook.Save("PivotField_AutoShowField_Example.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


