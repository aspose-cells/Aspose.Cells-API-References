---
title: "Clase ShapePropertyCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.ShapePropertyCollection. Esta clase especifica las propiedades visuales de la forma para un elemento de gráfico o forma"
type: docs
url: /es/net/aspose.cells.drawing/shapepropertycollection/
---
## ShapePropertyCollection class

Esta clase especifica las propiedades de forma visual para un elemento o forma de gráfico.

```csharp
public class ShapePropertyCollection
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Format3D](../../aspose.cells.drawing/shapepropertycollection/format3d/) { get; } | Representa un objeto [`Format3D`](./format3d/) que especifica las propiedades de forma 3D para el elemento de gráfico o forma. |
| [GlowEffect](../../aspose.cells.drawing/shapepropertycollection/gloweffect/) { get; } | Representa un objeto [`GlowEffect`](./gloweffect/) que especifica el efecto de resplandor para el elemento de gráfico o forma. |
| [ShadowEffect](../../aspose.cells.drawing/shapepropertycollection/shadoweffect/) { get; } | Representa un objeto [`ShadowEffect`](./shadoweffect/) que especifica el efecto de sombra para el elemento de gráfico o forma. |
| [SoftEdgeRadius](../../aspose.cells.drawing/shapepropertycollection/softedgeradius/) { get; set; } | Obtiene y establece el radio de desenfoque a aplicar en los bordes, en unidades de puntos. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [ClearFormat3D](../../aspose.cells.drawing/shapepropertycollection/clearformat3d/)() | Borra las propiedades de forma 3D de la forma. |
| [ClearGlowEffect](../../aspose.cells.drawing/shapepropertycollection/cleargloweffect/)() | Borra el efecto de resplandor de la forma. |
| [ClearShadowEffect](../../aspose.cells.drawing/shapepropertycollection/clearshadoweffect/)() | Borra el efecto de sombra del elemento de gráfico o forma. |
| [HasFormat3D](../../aspose.cells.drawing/shapepropertycollection/hasformat3d/)() | Indica si la forma tiene datos de formato 3D. |
| [HasGlowEffect](../../aspose.cells.drawing/shapepropertycollection/hasgloweffect/)() | Indica si la forma tiene datos de efecto de resplandor. |
| [HasShadowEffect](../../aspose.cells.drawing/shapepropertycollection/hasshadoweffect/)() | Indica si la forma tiene datos de efecto de sombra. |

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassShapePropertyCollectionDemo
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

            // Establece los colores de la serie
            series.Area.BackgroundColor = Color.Blue;
            series.Area.ForegroundColor = Color.Blue;
            series.Border.Color = Color.Blue;

            // Guarda el libro de trabajo
            workbook.Save("ShapePropertyCollectionDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


