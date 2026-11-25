---
title: "ChartTextFrame.IsResizeShapeToFitText"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ChartTextFrame. Ottiene o imposta se una forma deve adattarsi automaticamente per contenere completamente il testo descritto al suo interno. L'adattamento automatico avviene quando il testo all'interno di una forma viene scalato per contenere tutto il testo."
type: docs
url: /it/net/aspose.cells.charts/charttextframe/isresizeshapetofittext/
---
## ChartTextFrame.IsResizeShapeToFitText property

Ottiene o imposta se una forma deve adattarsi automaticamente per contenere completamente il testo descritto al suo interno. L'adattamento automatico avviene quando il testo all'interno di una forma viene scalato per contenere tutto il testo.

```csharp
public bool IsResizeShapeToFitText { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class ChartTextFramePropertyIsResizeShapeToFitTextDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook(FileFormatType.Xlsx);
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["A3"].PutValue("Category 3");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);

            // Aggiungi un grafico a colonne
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Imposta i dati della serie
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Accedi alle etichette dei dati
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowValue = true;
            dataLabels.Position = LabelPositionType.Center;

            // Dimostra la proprietà IsResizeShapeToFitText
            foreach (ChartPoint point in chart.NSeries[0].Points)
            {
                // Disabilita il ridimensionamento automatico della forma per adattare il testo
                point.DataLabels.IsResizeShapeToFitText = false;
                
                // Imposta una larghezza personalizzata più piccola di quella normalmente necessaria per il testo
                point.DataLabels.Width = 50;
            }

            // Salva la cartella di lavoro
            workbook.Save("ChartTextFramePropertyIsResizeShapeToFitTextDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


