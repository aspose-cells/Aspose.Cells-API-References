---
title: "Bevel.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Bevel. Ottiene e imposta il tipo di bevel predefinito"
type: docs
url: /it/net/aspose.cells.drawing/bevel/type/
---
## Bevel.Type property

Ottiene e imposta il tipo di smussatura predefinito.

```csharp
public BevelPresetType Type { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class BevelPropertyTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Aggiungi un grafico
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta i dati del grafico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Ottieni la prima serie
            Aspose.Cells.Charts.Series series = chart.NSeries[0];

            // Imposta il colore della serie
            series.Area.ForegroundColor = Color.Blue;

            // Configura il formato 3D e le proprietà del bevel
            Format3D format3D = series.ShapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;

            // Dimostra l'uso della proprietà Type
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Width = 5;
            topBevel.Height = 2;

            // Salva la cartella di lavoro
            workbook.Save("BevelPropertyTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* enum [BevelPresetType](../../bevelpresettype/)
* class [Bevel](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


