---
title: "PivotField.ShowValuesSetting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField-egenskap. Hämtar inställningarna för att visa värden när beräkningen ShowDataAs används"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/showvaluessetting/
---
## PivotField.ShowValuesSetting property

Hämtar inställningarna för att visa värden som när beräkningen ShowDataAs är i bruk.

```csharp
public PivotShowValuesSetting ShowValuesSetting { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyShowValuesSettingDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 1000;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 2000;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 3000;
            cells["A5"].Value = "Apple";
            cells["B5"].Value = 1500;
            cells["A6"].Value = "Orange";
            cells["B6"].Value = 2500;
            cells["A7"].Value = "Banana";
            cells["B7"].Value = 3500;

            // Skapa pivottabell
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B7", "C10", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Lägg till rad- och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[0];
            
            // Konfigurera ShowValuesSetting för att visas som procent av totalen
            dataField.ShowValuesSetting.CalculationType = PivotFieldDataDisplayFormat.PercentageOfTotal;
            
            // Beräkna och uppdatera pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Spara arbetsboken
            workbook.Save("PivotFieldShowValuesSettingDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotShowValuesSetting](../../pivotshowvaluessetting/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


