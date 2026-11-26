---
title: "Series.ShapeProperties"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Obtiene el objeto ShapePropertyCollection que contiene las propiedades visuales de forma de la Serie"
type: docs
url: /es/net/aspose.cells.charts/series/shapeproperties/
---
## Series.ShapeProperties property

Obtiene el objeto [`ShapePropertyCollection`](../../../aspose.cells.drawing/shapepropertycollection/) que contiene las propiedades visuales de forma de la Serie.

```csharp
public ShapePropertyCollection ShapeProperties { get; }
```

### Ejemplos

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

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer datos del gráfico
            chart.NSeries.Add("Sheet1!B2:B4", true);
            chart.NSeries.CategoryData = "Sheet1!A2:A4";

            // Obtener la primera serie y sus propiedades de forma
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Configura el formato 3D y el bisel
            Format3D format3D = shapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;
            topBevel.Type = BevelPresetType.Circle;
            topBevel.Height = 2;
            topBevel.Width = 5;

            // Configurar material e iluminación
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 20;

            // Establece los colores de la serie
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            // Guarda el libro de trabajo
            workbook.Save("SeriesShapePropertiesDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [ShapePropertyCollection](../../../aspose.cells.drawing/shapepropertycollection/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


