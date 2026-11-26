---
title: "ShapePropertyCollection.HasGlowEffect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ShapePropertyCollection método. Indica si la forma tiene datos de efecto de resplandor"
type: docs
url: /es/net/aspose.cells.drawing/shapepropertycollection/hasgloweffect/
---
## ShapePropertyCollection.HasGlowEffect method

Indica si la forma tiene datos de efecto de resplandor.

```csharp
public bool HasGlowEffect()
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;
    using System;

    public class ShapePropertyCollectionMethodHasGlowEffectDemo
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

            GlowEffect glowEffect = shapeProperties.GlowEffect;
            glowEffect.Size = 30;
            glowEffect.Color.Color = Color.Red;

            Console.WriteLine("Shape has glow effect: " + shapeProperties.HasGlowEffect());
                       

            // Guardar el resultado
            workbook.Save("ShapePropertyCollectionMethodHasGlowEffectDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


