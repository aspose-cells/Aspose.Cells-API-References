---
title: "PivotTable.RowHeaderCaption"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotTable-egenskap. Hämtar och anger anpassad rubrik för radhuvudet i denna pivottabell"
type: docs
url: /sv/net/aspose.cells.pivot/pivottable/rowheadercaption/
---
## PivotTable.RowHeaderCaption property

Hämtar och anger anpassad rubrik för radhuvudet i denna PivotTable.

```csharp
public string RowHeaderCaption { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyRowHeaderCaptionDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till dataarbetsblad
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Name = "Data";
            
            // Lägg till exempeldata
            var cells = dataSheet.Cells;
            cells["A1"].PutValue("State");
            cells["B1"].PutValue("City");
            cells["C1"].PutValue("Population");
            
            cells["A2"].PutValue("TN");
            cells["B2"].PutValue("Chennai");
            cells["C2"].PutValue("50");
            
            cells["A3"].PutValue("KL");
            cells["B3"].PutValue("Cochin");
            cells["C3"].PutValue("70");
            
            // Lägg till pivottabell-ark
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            
            // Lägg till pivottabell och hämta dess index
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Data!A1:C3", 
                "A3", 
                "PivotTable");
            
            // Hämta pivottabellinstansen
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Konfigurera pivottabell
            pivotTable.RowHeaderCaption = "State"; // Demonstrating RowHeaderCaption property
            pivotTable.AddFieldToArea(PivotFieldType.Row, "State");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Population");
            
            // Spara arbetsboken
            workbook.Save("PivotTableWithRowHeaderCaption.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


