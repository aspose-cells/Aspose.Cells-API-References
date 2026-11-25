---
title: "Area.FillFormat"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Area. Rappresenta un oggetto FillFormat che contiene le proprietà di formattazione di riempimento per il grafico o la forma specificati"
type: docs
url: /it/net/aspose.cells.drawing/area/fillformat/
---
## Area.FillFormat property

Rappresenta un oggetto `FillFormat` che contiene le proprietà di formattazione di riempimento per il grafico o la forma specificati.

```csharp
public FillFormat FillFormat { get; }
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
    public class AreaPropertyFillFormatDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio per il grafico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Imposta l'intervallo dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni il terzo punto della prima serie
            ChartPoint point = chart.NSeries[0].Points[2];
            
            // Imposta le proprietà del formato di riempimento
            point.Area.FillFormat.Pattern = FillPattern.DashedHorizontal;
            point.Area.FillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.Horizontal, 2);

            // Salva la cartella di lavoro
            workbook.Save("FillFormatDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [FillFormat](../../fillformat/)
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


