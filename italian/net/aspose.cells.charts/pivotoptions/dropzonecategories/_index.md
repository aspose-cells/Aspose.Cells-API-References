---
title: "PivotOptions.DropZoneCategories"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "PivotOptions property. Specifica se un controllo per ogni campo della PivotTable sull'asse della riga della PivotTable di origine appare sul grafico quando dropZonesVisible è impostato su true"
type: docs
url: /it/net/aspose.cells.charts/pivotoptions/dropzonecategories/
---
## PivotOptions.DropZoneCategories property

Specifica se un controllo per ogni campo della PivotTable sull'asse delle righe della PivotTable di origine appare sul grafico quando dropZonesVisible è impostato su true.

```csharp
public bool DropZoneCategories { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class PivotOptionsPropertyDropZoneCategoriesDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi un foglio di lavoro e alcuni dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            
            // Aggiungi un grafico che utilizza i dati pivot
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Accedi alle opzioni pivot dal grafico
            PivotOptions options = chart.PivotOptions;
            
            // Dimostra la proprietà DropZoneCategories
            options.DropZoneCategories = true;
            Console.WriteLine("DropZoneCategories enabled: " + options.DropZoneCategories);
            
            // Salva la cartella di lavoro
            workbook.Save("PivotOptionsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [PivotOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


