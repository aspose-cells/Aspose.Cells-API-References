---
title: "PivotField.ShowInOutlineForm"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Hämtar eller anger ett värde som indikerar om detta radfält använder konturlayout. Gäller endast radfält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/showinoutlineform/
---
## PivotField.ShowInOutlineForm property

Hämtar eller anger ett värde som visar om detta radfält använder konturlayout. Gäller endast radfält.

```csharp
public bool ShowInOutlineForm { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowInOutlineFormDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok med exempeldata
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Apple";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["A5"].Value = "Orange";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 20;
            worksheet.Cells["B5"].Value = 25;

            // Skapa pivottabell
            int index = worksheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Lägg till radfält och demonstrera ShowInOutlineForm
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            PivotField rowField = pivotTable.RowFields[0];
            
            // Ställ in ShowInOutlineForm till false
            rowField.ShowInOutlineForm = false;
            
            // Lägg till datafält
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Uppdatera och beräkna pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotFieldShowInOutlineFormDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


