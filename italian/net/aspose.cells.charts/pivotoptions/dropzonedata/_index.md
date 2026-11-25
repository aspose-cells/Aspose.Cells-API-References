---
title: "PivotOptions.DropZoneData"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotOptions property. Specifica se un controllo per ogni campo della PivotTable sull'asse dei dati della PivotTable di origine appare sul grafico quando dropZonesVisible è impostato su true"
type: docs
url: /it/net/aspose.cells.charts/pivotoptions/dropzonedata/
---
## PivotOptions.DropZoneData property

Specifica se un controllo per ogni campo della PivotTable sull'asse dei dati della PivotTable di origine appare sul grafico quando dropZonesVisible è impostato su true.

```csharp
public bool DropZoneData { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneDataDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Dati di esempio per la tabella pivot
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Books");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Books");
            worksheet.Cells["B4"].PutValue(1500);

            // Crea tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "D1", "SalesPivot");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crea un grafico collegato alla tabella pivot
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "SalesPivot";

            // Configura le opzioni pivot con DropZoneData abilitato
            PivotOptions pivotOptions = chart.PivotOptions;
            pivotOptions.DropZoneData = true;
            pivotOptions.DropZonesVisible = true;

            // Salva il risultato
            workbook.Save("PivotOptionsDropZoneDataDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


