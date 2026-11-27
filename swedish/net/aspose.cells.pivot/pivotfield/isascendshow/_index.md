---
title: "PivotField.IsAscendShow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Anger om det angivna PivotTable-fältet automatiskt visas i stigande ordning"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/isascendshow/
---
## PivotField.IsAscendShow property

Indikerar om det angivna pivåtabellfältet automatiskt visas i stigande ordning.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.IsTop property or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAscendShow { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället egenskapen PivotField.Top10AutoShowSettings.IsTop eller metoden PivotField.Top10AutoShow(). Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAscendShowDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 200;
            worksheet.Cells["B4"].Value = 150;

            // Lägg till pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];
            
            // Ställ in egenskapen IsAscendShow
            rowField.IsAscendShow = true;
            Console.WriteLine("IsAscendShow (Row Field): " + rowField.IsAscendShow);
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[0];
            
            // Ställ in egenskapen IsAscendShow
            dataField.IsAscendShow = false;
            Console.WriteLine("IsAscendShow (Data Field): " + dataField.IsAscendShow);
            
            // Uppdatera pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


