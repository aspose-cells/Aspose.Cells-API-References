---
title: "Clase Format3D"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Format3D. Esta clase especifica las propiedades de forma 3D para un elemento de gráfico o forma"
type: docs
url: /es/net/aspose.cells.drawing/format3d/
---
## Format3D class

Esta clase especifica las propiedades de forma 3D para un elemento de gráfico o forma.

```csharp
public class Format3D
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [LightingAngle](../../aspose.cells.drawing/format3d/lightingangle/) { get; set; } | Obtiene y establece el ángulo de iluminación. Rango de 0 a 359,9 grados. |
| [SurfaceLightingType](../../aspose.cells.drawing/format3d/surfacelightingtype/) { get; set; } | Obtiene y establece el tipo de iluminación que se aplicará a la escena de la forma. El valor predeterminado es LightRigType.ThreePoint. |
| [SurfaceMaterialType](../../aspose.cells.drawing/format3d/surfacematerialtype/) { get; set; } | Obtiene y establece el tipo de material que se combina con las propiedades de iluminación para dar el aspecto y la sensación final de una forma. El valor predeterminado es PresetMaterialType.WarmMatte. |
| [TopBevel](../../aspose.cells.drawing/format3d/topbevel/) { get; } | Obtiene el objeto [`Bevel`](../bevel/) que contiene las propiedades asociadas con la definición de un bisel en la cara superior o frontal de una forma. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [HasTopBevelData](../../aspose.cells.drawing/format3d/hastopbeveldata/)() | Indica si la forma tiene datos de bisel superior. |

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class Format3DDemo
    {
        public static void RunDemo()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = sheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 20, 10);
            Chart chart = sheet.Charts[chartIndex];

            // Agregar series al gráfico
            chart.NSeries.Add("A1:A4", true);

            // Acceder a la primera serie
            Series series = chart.NSeries[0];

            // Acceder al formato 3D de la serie
            Format3D format3D = series.ShapeProperties.Format3D;

            // Establecer las propiedades del formato 3D
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 45.0;

            // Comprobar si la forma tiene datos de bisel superior
            if (format3D.HasTopBevelData())
            {
                Bevel topBevel = format3D.TopBevel;
                Console.WriteLine("Top Bevel Width: " + topBevel.Width);
                Console.WriteLine("Top Bevel Height: " + topBevel.Height);
            }

            // Guarda el libro de trabajo
            workbook.Save("Format3DDemo.xlsx");
            workbook.Save("Format3DDemo.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


