---
title: "Enumeración SvgEmbeddedFontType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Rendering.SvgEmbeddedFontType. Representa el tipo de fuente incrustada en la imagen Svg"
type: docs
url: /es/net/aspose.cells.rendering/svgembeddedfonttype/
---
## SvgEmbeddedFontType enumeration

Representa el tipo de fuente incrustada en una imagen Svg.

```csharp
public enum SvgEmbeddedFontType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | No incrustar fuente. |
| Woff | `1` | Incrustar fuente WOFF. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassSvgEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries.CategoryData = "A1:A3";

            // Configurar opciones de imagen SVG
            SvgImageOptions svgOptions = new SvgImageOptions
            {
                EmbeddedFontType = SvgEmbeddedFontType.Woff,
                FitToViewPort = true,
                CssPrefix = "chart-prefix"
            };

            // Guardar el gráfico como SVG con fuente WOFF incrustada
            chart.ToImage("output_chart.svg", svgOptions);

            Console.WriteLine("SVG with embedded WOFF font generated successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


