---
title: "ShapePropertyCollection.HasShadowEffect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ShapePropertyCollection método. Indica si la forma tiene datos de efecto de sombra"
type: docs
url: /es/net/aspose.cells.drawing/shapepropertycollection/hasshadoweffect/
---
## ShapePropertyCollection.HasShadowEffect method

Indica si la forma tiene datos de efecto de sombra.

```csharp
public bool HasShadowEffect()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ShapePropertyCollectionMethodHasShadowEffectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un gráfico de ejemplo
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category 1");
            worksheet.Cells["A2"].PutValue("Category 2");
            worksheet.Cells["B1"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);

            chart.NSeries.Add("B1:B2", true);
            chart.NSeries.CategoryData = "A1:A2";

            // Accede a las propiedades de forma de la primera serie
            Aspose.Cells.Charts.Series series = chart.NSeries[0];
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Configura el formato 3D y el bisel
            Format3D format3D = shapeProperties.Format3D;
            Bevel topBevel = format3D.TopBevel;

            topBevel.Type = BevelPresetType.Circle;
            topBevel.Height = 2;
            topBevel.Width = 5;

            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 20;

            ShadowEffect shadowEffect = shapeProperties.ShadowEffect;
            shadowEffect.Size = 1.5;
            shadowEffect.Color.Color = Color.Red;
            shadowEffect.Angle = 180;

            // Establece los colores de la serie
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            Console.WriteLine($"Shape has shadow effect after: {shapeProperties.HasShadowEffect()}");

            // Guardar el resultado
            workbook.Save("ShapePropertyCollectionMethodHasShadowEffectDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


