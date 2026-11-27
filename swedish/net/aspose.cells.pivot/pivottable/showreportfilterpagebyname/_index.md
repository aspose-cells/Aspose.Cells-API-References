---
title: "PivotTable.ShowReportFilterPageByName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-metod. Visa alla rapportfilter-sidor enligt PivotFields namn. PivotField måste vara placerad i PageFields"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/showreportfilterpagebyname/
---
## PivotTable.ShowReportFilterPageByName method

Visa alla rapportfilter‑sidor enligt PivotField:s namn, PivotField måste vara placerad i PageFields.

```csharp
public void ShowReportFilterPageByName(string fieldName)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldName | String | Namnet på PivotField |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowReportFilterPageByNameWithStringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok från käll‑Excel‑filen
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till exempeldata för pivottabell
            var cells = sheet.Cells;
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
            
            // Skapa pivottabell
            int index = sheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];
            
            // Lägg till rad- och datafält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
            
            // Lägg till sidfält
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Fruit");
            pivotTable.PageFields[0].Name = "FruitFilter";
            
            // Uppdatera pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Visa rapportfilter-sidor efter namn
            pivotTable.ShowReportFilterPageByName("FruitFilter");
            
            // Spara arbetsboken
            workbook.Save("PivotTableShowReportFilterPageByNameDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


