---
title: "Enumeración BevelPresetType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.BevelPresetType. Representa una configuración predefinida para un tipo de bisel que puede aplicarse a una forma en 3D"
type: docs
url: /es/net/aspose.cells.drawing/bevelpresettype/
---
## BevelPresetType enumeration

Representa un preset para un tipo de bisel que puede aplicarse a una forma en 3D.

```csharp
public enum BevelPresetType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Sin bisel |
| Angle | `1` | Ángulo |
| ArtDeco | `2` | Art déco |
| Circle | `3` | Círculo |
| Convex | `4` | Convexo |
| CoolSlant | `5` | Inclinación fresca |
| Cross | `6` | Cruz |
| Divot | `7` | Hueco |
| HardEdge | `8` | Borde duro |
| RelaxedInset | `9` | Inserción relajada |
| Riblet | `10` | Estría |
| Slope | `11` | Pendiente |
| SoftRound | `12` | Redondez suave |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Charts;
    using System;

    public class BevelPresetTypeDemo
    {
        public static void BevelPresetTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column3D, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer el rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", true);

            // Accede al título del gráfico y establece su texto
            chart.Title.Text = "Sample Chart with Bevel";

            // Acceder al área de trazado del gráfico
            PlotArea plotArea = chart.PlotArea;

            // Accede a las propiedades de forma del área de trazado
            ShapePropertyCollection shapeProperties = plotArea.ShapeProperties;

            
            // Accede a las propiedades de formato 3D
            Format3D format3D = shapeProperties.Format3D;

            // Accede a las propiedades del bisel superior
            Bevel topBevel = format3D.TopBevel;

            // Establece el tipo de bisel a "Ángulo"
            topBevel.Type = BevelPresetType.Angle;

            // Establece el ancho y la altura del bisel
            topBevel.Width = 10;
            topBevel.Height = 10;

            // Guarda el libro de trabajo
            workbook.Save("BevelPresetTypeExample.xlsx");
            workbook.Save("BevelPresetTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


