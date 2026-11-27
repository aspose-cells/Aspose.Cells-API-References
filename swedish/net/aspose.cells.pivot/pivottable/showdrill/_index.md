---
title: "PivotTable.ShowDrill"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Hämtar och anger om expand/collapse-knappar visas"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showdrill/
---
## PivotTable.ShowDrill property

Hämtar och anger om expandera/komprimera‑knappar ska visas.

```csharp
public bool ShowDrill { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowDrillDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad och fyll i med exempeldata
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Name = "Pivot";
            sheet.Cells["A1"].Value = "Category";
            sheet.Cells["B1"].Value = "Value";
            sheet.Cells["A2"].Value = "A";
            sheet.Cells["B2"].Value = 100;
            sheet.Cells["A3"].Value = "B";
            sheet.Cells["B3"].Value = 200;
            sheet.Cells["A4"].Value = "A";
            sheet.Cells["B4"].Value = 150;

            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Konfigurera pivottabell
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Aktivera drilldown och visa drillindikatorer
            pivotTable.EnableDrilldown = true;
            pivotTable.ShowDrill = true;
            
            // Uppdatera och beräkna data
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotTableShowDrillDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


