---
title: "PivotOptions.DropZonesVisible"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotOptions property. Specifica se eventuali controlli pivot possono apparire sul grafico pivot"
type: docs
url: /it/net/aspose.cells.charts/pivotoptions/dropzonesvisible/
---
## PivotOptions.DropZonesVisible property

Specifica se dei controlli pivot possono apparire sul grafico pivot.

```csharp
public bool DropZonesVisible { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZonesVisibleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crea un grafico collegato alla tabella pivot
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "PivotTable1";

            // Configura le opzioni pivot con DropZonesVisible
            PivotOptions pivotOptions = chart.PivotOptions;
            pivotOptions.DropZonesVisible = true;

            workbook.Save("PivotOptionsDropZonesVisibleDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


