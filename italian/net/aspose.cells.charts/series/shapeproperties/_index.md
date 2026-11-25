---
title: "Series.ShapeProperties"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Series. Ottiene l'oggetto ShapePropertyCollection che contiene le proprietà visive della forma della Series"
type: docs
url: /it/net/aspose.cells.charts/series/shapeproperties/
---
## Series.ShapeProperties property

Ottiene l'oggetto [`ShapePropertyCollection`](../../../aspose.cells.drawing/shapepropertycollection/) che contiene le proprietà visive della forma della Series.

```csharp
public ShapePropertyCollection ShapeProperties { get; }
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
    public class SeriesPropertyShapePropertiesDemo
    {
        public static void Run()
        {
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

            // Aggiungi grafico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Imposta i dati del grafico
            chart.NSeries.Add("Sheet1!B2:B4", true);
            chart.NSeries.CategoryData = "Sheet1!A2:A4";

            // Ottieni la prima serie e le sue proprietà di forma
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Configura il formato 3D e lo smusso
            Format3D format3D = shapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Height = 2;
            topBevel.Width = 5;

            // Configura materiale e illuminazione
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 20;

            // Imposta i colori della serie
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            // Salva la cartella di lavoro
            workbook.Save("SeriesShapePropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Vedi anche

* class [ShapePropertyCollection](../../../aspose.cells.drawing/shapepropertycollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


