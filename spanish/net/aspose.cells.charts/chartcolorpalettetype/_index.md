---
title: "Enum ChartColorPaletteType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.ChartColorPaletteType enum. Enumera todas las Paletas Monocromáticas usadas en un gráfico de Excel"
type: docs
url: /es/net/aspose.cells.charts/chartcolorpalettetype/
---
## ChartColorPaletteType enumeration

Enumera todas las paletas monocromáticas usadas en un gráfico de Excel.

```csharp
public enum ChartColorPaletteType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| MonochromaticPalette1 | `1` | gradiente de color de tema accent1, de oscuro a claro. |
| MonochromaticPalette2 | `2` | gradiente de color de tema accent2, de oscuro a claro. |
| MonochromaticPalette3 | `3` | gradiente de color de tema accent3, de oscuro a claro. |
| MonochromaticPalette4 | `4` | gradiente de color de tema accent4, de oscuro a claro. |
| MonochromaticPalette5 | `5` | gradiente de color de tema accent5, de oscuro a claro. |
| MonochromaticPalette6 | `6` | gradiente de color de tema accent6, de oscuro a claro. |
| MonochromaticPalette7 | `7` | gradiente de color de tema accent7. |
| MonochromaticPalette8 | `8` | gradiente de color de tema accent1, de claro a oscuro. |
| MonochromaticPalette9 | `9` | gradiente de color de tema accent2, de claro a oscuro. |
| MonochromaticPalette10 | `10` | gradiente de color de tema accent3, de claro a oscuro. |
| MonochromaticPalette11 | `11` | gradiente de color de tema accent4, de claro a oscuro. |
| MonochromaticPalette12 | `12` | gradiente de color de tema accent5, de claro a oscuro. |
| MonochromaticPalette13 | `13` | gradiente de color de tema accent6, de claro a oscuro. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassChartColorPaletteTypeDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar un gráfico de ejemplo para demostrar la paleta de colores
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];

                // Demostrar el uso de diferentes valores del enum ChartColorPaletteType
                ChartColorPaletteType palette1 = ChartColorPaletteType.MonochromaticPalette1;
                ChartColorPaletteType palette5 = ChartColorPaletteType.MonochromaticPalette5;
                ChartColorPaletteType palette8 = ChartColorPaletteType.MonochromaticPalette8;

                // Mostrar los valores del enum
                Console.WriteLine($"MonochromaticPalette1 value: {(int)palette1}");
                Console.WriteLine($"MonochromaticPalette5 value: {(int)palette5}");
                Console.WriteLine($"MonochromaticPalette8 value: {(int)palette8}");

                // Guarda el libro de trabajo
                workbook.Save("ChartColorPaletteTypeDemo.xlsx");
                Console.WriteLine("ChartColorPaletteType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ChartColorPaletteType: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


