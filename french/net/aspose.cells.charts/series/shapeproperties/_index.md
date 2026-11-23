---
title: "Series.ShapeProperties"
second_title: "Référence de l'API Aspose.Cells pour .NET"
description: "Propriété Series. Obtient l'objet ShapePropertyCollection qui contient les propriétés visuelles de forme de la série"
type: docs
url: /fr/net/aspose.cells.charts/series/shapeproperties/
---
## Series.ShapeProperties property

Obtient l'objet [`ShapePropertyCollection`](../../../aspose.cells.drawing/shapepropertycollection/) qui contient les propriétés visuelles de forme de la série.

```csharp
public ShapePropertyCollection ShapeProperties { get; }
```

### Exemples

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

            // Ajoutez des données d'exemple
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Ajouter un graphique
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Définir les données du graphique
            chart.NSeries.Add("Sheet1!B2:B4", true);
            chart.NSeries.CategoryData = "Sheet1!A2:A4";

            // Obtenir la première série et ses propriétés de forme
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Configurer le format 3D et le biseau
            Format3D format3D = shapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Height = 2;
            topBevel.Width = 5;

            // Configurer le matériau et l'éclairage
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 20;

            // Définir les couleurs des séries
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            // Enregistrez le classeur
            workbook.Save("SeriesShapePropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Voir aussi

* class [ShapePropertyCollection](../../../aspose.cells.drawing/shapepropertycollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


