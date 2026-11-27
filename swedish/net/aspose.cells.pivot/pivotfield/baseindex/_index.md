---
title: "PivotField.BaseIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField egenskap. Representerar indexet i källpivottfälten."
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/baseindex/
---
## PivotField.BaseIndex property

Representerar indexet i källpivotfälten.

```csharp
public int BaseIndex { get; set; }
```

### Anmärkningar

OBS: Denna setter för denna egenskap är nu föråldrad. Denna setter för denna egenskap kommer att tas bort 12 månader senare från och med september 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyBaseIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[wb.Worksheets.Add()];
            ws.Name = "PivotData";
            
            // Exempeldata
            ws.Cells["A1"].PutValue("Category");
            ws.Cells["B1"].PutValue("Quarter");
            ws.Cells["C1"].PutValue("Sales");
            
            ws.Cells["A2"].PutValue("Electronics");
            ws.Cells["A3"].PutValue("Electronics");
            ws.Cells["A4"].PutValue("Clothing");
            ws.Cells["A5"].PutValue("Clothing");
            
            ws.Cells["B2"].PutValue("Q1");
            ws.Cells["B3"].PutValue("Q2");
            ws.Cells["B4"].PutValue("Q1");
            ws.Cells["B5"].PutValue("Q2");
            
            ws.Cells["C2"].PutValue(1000);
            ws.Cells["C3"].PutValue(1200);
            ws.Cells["C4"].PutValue(800);
            ws.Cells["C5"].PutValue(900);

            // Skapa pivottabell - åtgärdad genom att hämta PivotTable från indexet
            int pivotIndex = ws.PivotTables.Add("=PivotData!A1:C5", "E3", "PivotTable1");
            PivotTable pt = ws.PivotTables[pivotIndex];
            
            // Lägg till radfält
            int rowIndex = pt.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pt.RowFields[rowIndex];
            
            // Lägg till kolumnfält (kommer att användas som basfält)
            int colIndex = pt.AddFieldToArea(PivotFieldType.Column, "Quarter");
            PivotField quarterField = pt.ColumnFields[colIndex];
            
            // Lägg till datafält med normal beräkning
            int dataIndex = pt.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pt.DataFields[dataIndex];
            dataField.Function = ConsolidationFunction.Sum;
            
            // Lägg till ett andra datafält som visar skillnad från föregående kvartal
            int diffIndex = pt.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField diffField = pt.DataFields[diffIndex];
            diffField.DisplayName = "QoQ Difference";
            diffField.ShowValuesAs(
                PivotFieldDataDisplayFormat.DifferenceFrom, 
                quarterField.BaseIndex, 
                PivotItemPositionType.Previous,
                0);
            
            // Beräkna och spara
            wb.CalculateFormula();
            wb.Save("PivotTableWithBaseIndexDemo.xlsx");
        }
    }
}
```

### Se även

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


