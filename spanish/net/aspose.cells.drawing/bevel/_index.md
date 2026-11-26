---
title: "Clase Bevel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.Bevel. Representa un bisel de una forma"
type: docs
url: /es/net/aspose.cells.drawing/bevel/
---
## Bevel class

Representa un bisel de una forma

```csharp
public class Bevel
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Height](../../aspose.cells.drawing/bevel/height/) { get; set; } | Obtiene y establece la altura del bisel, o cuán lejos sobre la forma se aplica. En unidades de puntos. |
| [Type](../../aspose.cells.drawing/bevel/type/) { get; set; } | Obtiene y establece el tipo de bisel predefinido. |
| [Width](../../aspose.cells.drawing/bevel/width/) { get; set; } | Obtiene y establece el ancho del bisel, o cuán lejos dentro de la forma se aplica. En unidades de puntos. |

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class BevelDemo
    {
        public static void RunDemo()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            workbook.CalculateFormula();

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar series de datos al gráfico
            chart.NSeries.Add("A1:B4", true);

            // Acceder al área de trazado del gráfico
            ChartFrame plotArea = chart.PlotArea;

            // Accede a las propiedades de forma del área de trazado
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            // Accede a las propiedades de formato 3D
            Format3D format3D = shapeProperties.Format3D;

            // Accede a las propiedades del bisel superior
            Bevel topBevel = format3D.TopBevel;

            // Establezca el ancho, la altura y el tipo del bisel
            topBevel.Width = 10.0;
            topBevel.Height = 5.0;
            topBevel.Type = BevelPresetType.Circle;

            // Establezca otras propiedades de formato 3D
            format3D.SurfaceMaterialType = PresetMaterialType.WarmMatte;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;
            format3D.LightingAngle = 45.0;

            // Guarda el libro de trabajo
            workbook.Save("BevelDemo.xlsx");
            workbook.Save("BevelDemo.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


