---
title: "Enumeración LightRigType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.LightRigType. Representa una luz predefinida que se puede aplicar a una forma"
type: docs
url: /es/net/aspose.cells.drawing/lightrigtype/
---
## LightRigType enumeration

Representa una luz preestablecida derecha que se puede aplicar a una forma

```csharp
public enum LightRigType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Balanced | `0` | Equilibrado |
| BrightRoom | `1` | Sala brillante |
| Chilly | `2` | Frío |
| Contrasting | `3` | Contrastante |
| Flat | `4` | Plano |
| Flood | `5` | Inundación |
| Freezing | `6` | Congelante |
| Glow | `7` | Brillo |
| Harsh | `8` | Áspero |
| LegacyFlat1 | `9` | LegacyFlat1 |
| LegacyFlat2 | `10` | LegacyFlat2 |
| LegacyFlat3 | `11` | LegacyFlat3 |
| LegacyFlat4 | `12` | LegacyFlat4 |
| LegacyHarsh1 | `13` | LegacyHarsh1 |
| LegacyHarsh2 | `14` | LegacyHarsh2 |
| LegacyHarsh3 | `15` | LegacyHarsh3 |
| LegacyHarsh4 | `16` | LegacyHarsh4 |
| LegacyNormal1 | `17` | LegacyNormal1 |
| LegacyNormal2 | `18` | LegacyNormal2 |
| LegacyNormal3 | `19` | LegacyNormal3 |
| LegacyNormal4 | `20` | LegacyNormal4 |
| Morning | `21` | Mañana |
| Soft | `22` | Suave |
| Sunrise | `23` | Amanecer |
| Sunset | `24` | Atardecer |
| ThreePoint | `25` | Tres puntos |
| TwoPoint | `26` | Dos puntos |
| None | `27` | Sin configuración de luz. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class LightRigTypeDemo
    {
        public static void LightRigTypeExample()
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer el rango de datos del gráfico
            chart.SetChartDataRange("A1:B4", true);

            // Acceder a la primera serie del gráfico
            Series series = chart.NSeries[0];

            // Acceder a las propiedades de forma de la serie
            ShapePropertyCollection shapeProperties = series.ShapeProperties;

            // Comprobar si la serie tiene datos de formato 3D
            if (shapeProperties.HasFormat3D())
            {
                // Accede a las propiedades de formato 3D
                Format3D format3D = shapeProperties.Format3D;

                // Establecer el tipo de iluminación de superficie a Equilibrado
                format3D.SurfaceLightingType = LightRigType.Balanced;

                // Establecer el ángulo de iluminación
                format3D.LightingAngle = 45.0;
            }

            // Guarda el libro de trabajo
            workbook.Save("LightRigTypeExample.xlsx");
            workbook.Save("LightRigTypeExample.pdf");
            // Genere la salida de los resultados
            Console.WriteLine("LightRigType example applied and workbook saved as 'LightRigTypeExample.xlsx'.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


