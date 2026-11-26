---
title: "SvgImageOptions.CssPrefix"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SvgImageOptions. Obtiene y establece el prefijo del nombre css en svg; el valor predeterminado es una cadena vacía"
type: docs
url: /es/net/aspose.cells.rendering/svgimageoptions/cssprefix/
---
## SvgImageOptions.CssPrefix property

Obtiene y establece el prefijo del nombre CSS en SVG, el valor predeterminado es una cadena vacía.

```csharp
public string CssPrefix { get; set; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Rendering;
    using System;
    using System.IO;

    public class SvgImageOptionsPropertyCssPrefixDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["B1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue(2019);
            worksheet.Cells["A3"].PutValue(2020);
            worksheet.Cells["A4"].PutValue(2021);
            worksheet.Cells["A5"].PutValue(2022);

            worksheet.Cells["B2"].PutValue(4500);
            worksheet.Cells["B3"].PutValue(4900);
            worksheet.Cells["B4"].PutValue(5200);
            worksheet.Cells["B5"].PutValue(6100);

            // Crear un gráfico de líneas
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B5", true);

            // Crear opciones de imagen SVG
            SvgImageOptions svgOptions = new SvgImageOptions();

            // Mostrar el prefijo CSS actual
            Console.WriteLine("Current CssPrefix value: " + svgOptions.CssPrefix);

            // Establecer un nuevo prefijo CSS
            svgOptions.CssPrefix = "chart-prefix-";

            // Demostrar la generación de SVG con un prefijo CSS personalizado
            string outputPath = "output_chart.svg";
            chart.ToImage(outputPath, svgOptions);

            Console.WriteLine("Chart saved as SVG with custom CSS prefix.");
        }
    }
}
```

### Ver también

* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


