---
title: "PivotField.IsAutoShow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Anger om det angivna pivottabellfältet visas automatiskt"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/isautoshow/
---
## PivotField.IsAutoShow property

Anger om det angivna pivottabellfältet visas automatiskt.

```csharp
[Obsolete("Use  PivotField.Top10AutoShowSettings.IsAutoShow property  or PivotField.Top10AutoShow() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsAutoShow { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd i stället PivotField.Top10AutoShowSettings.IsAutoShow-egenskap eller PivotField.Top10AutoShow()-metod. Denna metod kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyIsAutoShowDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            worksheet.Cells["B4"].Value = 3000;

            // Lägg till pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            
            // Lägg till datafält och konfigurera IsAutoShow
            int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[dataFieldIndex];
            
            // Aktivera AutoShow och konfigurera inställningarna
            dataField.IsAutoShow = true;
            dataField.AutoShowCount = 2;
            dataField.AutoShowField = 0; // Index of the field to auto show
            dataField.IsAscendShow = true;
            
            // Beräkna data
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Skriv ut värdet för IsAutoShow-egenskapen
            Console.WriteLine("IsAutoShow property value: " + dataField.IsAutoShow);
            
            // Spara arbetsboken
            workbook.Save("PivotFieldPropertyIsAutoShowDemo_out.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


