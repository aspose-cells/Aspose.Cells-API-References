---
title: "Enum PresetMaterialType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.PresetMaterialType enum. Describe la apariencia de la superficie de una forma"
type: docs
url: /es/net/aspose.cells.drawing/presetmaterialtype/
---
## PresetMaterialType enumeration

Describe la apariencia superficial de una forma.

```csharp
public enum PresetMaterialType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Clear | `0` | Borrar |
| DarkEdge | `1` | Borde oscuro |
| Flat | `2` | Plano |
| LegacyMatte | `3` | Mate heredado |
| LegacyMetal | `4` | Metal heredado |
| LegacyPlastic | `5` | Plástico heredado |
| LegacyWireframe | `6` | Estructura de alambre heredada |
| Matte | `7` | Mate |
| Metal | `8` | Metal |
| Plastic | `9` | Plástico |
| Powder | `10` | Polvo |
| SoftEdge | `11` | Borde suave |
| SoftMetal | `12` | Metal suave |
| TranslucentPowder | `13` | Polvo translúcido |
| WarmMatte | `14` | Mate cálido |

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System;

namespace AsposeCellsExamples
{
    public class PresetMaterialTypeDemo
    {
        public static void PresetMaterialTypeExample()
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

            // Acceder a la primera serie del gráfico
            Series series = chart.NSeries[0];

            // Acceder al formato 3D de la serie
            Format3D format3D = series.ShapeProperties.Format3D;

            // Establecer el tipo de material de la superficie
            format3D.SurfaceMaterialType = PresetMaterialType.Metal;

            // Establecer otras propiedades 3D
            format3D.LightingAngle = 45;
            format3D.SurfaceLightingType = LightRigType.ThreePoint;

            // Guarda el libro de trabajo
            workbook.Save("PresetMaterialTypeExample.xlsx");

            // Genere la salida de los resultados
            Console.WriteLine("Chart with 3D format and PresetMaterialType applied has been created.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


