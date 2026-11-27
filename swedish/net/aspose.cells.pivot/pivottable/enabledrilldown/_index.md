---
title: "PivotTable.EnableDrilldown"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Anger om drilldown är aktiverat"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/enabledrilldown/
---
## PivotTable.EnableDrilldown property

Anger om drill‑down är aktiverat.

```csharp
public bool EnableDrilldown { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyEnableDrilldownDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till ett kalkylblad och fyll i med exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 100;
            worksheet.Cells["B3"].Value = 150;
            worksheet.Cells["B4"].Value = 200;

            // Skapa en pivottabell
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Konfigurera pivottabellens fält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            
            // Aktivera drilldown‑funktionalitet
            pivotTable.EnableDrilldown = true;
            
            // Spara arbetsboken
            workbook.Save("PivotTableEnableDrilldownDemo.xlsx");
            
            // Verifiera att egenskapen har satts
            Console.WriteLine("EnableDrilldown property is set to: " + pivotTable.EnableDrilldown);
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


