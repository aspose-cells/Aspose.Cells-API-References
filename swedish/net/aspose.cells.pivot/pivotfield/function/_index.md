---
title: "PivotField.Function"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PivotField egenskap. Representerar funktionen som används för att summera detta PivotTable-datafält"
type: docs
url: /sv/net/aspose.cells.pivot/pivotfield/function/
---
## PivotField.Function property

Representerar funktionen som används för att sammanfatta detta PivotTable-datfält.

```csharp
public ConsolidationFunction Function { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyFunctionDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Lägg till exempeldata
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "A";
            cells["B2"].Value = 100;
            cells["A3"].Value = "B";
            cells["B3"].Value = 120;
            cells["A4"].Value = "A";
            cells["B4"].Value = 80;
            cells["A5"].Value = "B";
            cells["B5"].Value = 60;

            // Skapa pivottabell
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];

            // Lägg till radfält
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");

            // Lägg till datafält och sätt funktionen till Max
            int fieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pivotTable.DataFields[fieldIndex];
            dataField.Function = ConsolidationFunction.Max;

            // Beräkna pivottabell
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Spara arbetsboken
            workbook.Save("PivotFieldFunctionDemo.xlsx");
        }
    }
}
```

### Se även

* enum [ConsolidationFunction](../../../aspose.cells/consolidationfunction/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


