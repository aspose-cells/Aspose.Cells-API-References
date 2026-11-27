---
title: "PivotField.AutoShowCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Representerar antalet översta eller nedersta objekt som automatiskt visas i det angivna PivotTable-fältet."
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/autoshowcount/
---
## PivotField.AutoShowCount property

Representerar antalet topp- eller bottenobjekt som automatiskt visas i det angivna pivåtabellfältet.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.AutoShowCount property or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int AutoShowCount { get; set; }
```

### Anmärkningar

OBS: Den här egenskapen är nu föråldrad. Använd istället PivotField.Top10AutoShowSettings.AutoShowCount-egenskapen eller PivotField.Top10AutoShow()-metoden. Denna metod kommer att tas bort 12 månader senare, från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyAutoShowCountDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
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
            cells["B6"].Value = 25;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B6", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Lägg till radfält och ställ in AutoShow-egenskaperna
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];
            rowField.AutoShowCount = 2;
            rowField.IsAutoShow = true;
            rowField.AutoShowField = 1; // Index of "Quantity" field (0-based)

            // Beräkna data och spara
            pivotTable.CalculateData();
            workbook.Save("PivotFieldAutoShowCountDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


