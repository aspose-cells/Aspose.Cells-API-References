---
title: "Classe PivotOptions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Charts.PivotOptions. Rappresenta un tipo complesso che specifica i controlli pivot che appaiono sul grafico"
type: docs
url: /it/net/aspose.cells.charts/pivotoptions/
---
## PivotOptions class

Rappresenta un tipo complesso che specifica i controlli pivot che appaiono sul grafico

```csharp
public class PivotOptions
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DropZoneCategories](../../aspose.cells.charts/pivotoptions/dropzonecategories/) { get; set; } | Specifica se un controllo per ogni campo della PivotTable sull'asse delle righe della PivotTable di origine appare sul grafico quando dropZonesVisible è impostato su true. |
| [DropZoneData](../../aspose.cells.charts/pivotoptions/dropzonedata/) { get; set; } | Specifica se un controllo per ogni campo della PivotTable sull'asse dei dati della PivotTable di origine appare sul grafico quando dropZonesVisible è impostato su true. |
| [DropZoneFilter](../../aspose.cells.charts/pivotoptions/dropzonefilter/) { get; set; } | Specifica se un controllo per ogni campo della PivotTable sull'asse della pagina della PivotTable di origine appare sul grafico quando dropZonesVisible è impostato su true. |
| [DropZoneSeries](../../aspose.cells.charts/pivotoptions/dropzoneseries/) { get; set; } | Specifica se un controllo per ogni campo della PivotTable sull'asse delle colonne della PivotTable di origine appare sul grafico quando dropZonesVisible è impostato su true. |
| [DropZonesVisible](../../aspose.cells.charts/pivotoptions/dropzonesvisible/) { get; set; } | Specifica se dei controlli pivot possono apparire sul grafico pivot. |
| [ShowExpandCollapseFieldButtons](../../aspose.cells.charts/pivotoptions/showexpandcollapsefieldbuttons/) { get; set; } | Ottiene o imposta un valore che indica se mostrare i pulsanti di espansione o compressione dei campi |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotOptionsDemo
    {
        public static void PivotOptionsExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati per la tabella pivot
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

            // Aggiungi una tabella pivot
            int pivotIndex = worksheet.PivotTables.Add("=A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.PivotSource = "PivotTable1";

            // Accedi alle PivotOptions del grafico
            PivotOptions pivotOptions = chart.PivotOptions;

            // Imposta le proprietà di PivotOptions
            pivotOptions.DropZoneFilter = true;
            pivotOptions.DropZoneCategories = true;
            pivotOptions.DropZoneData = true;
            pivotOptions.DropZoneSeries = true;
            pivotOptions.DropZonesVisible = true;

            // Salva la cartella di lavoro
            workbook.Save("PivotOptionsExample.xlsx");

            return;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


