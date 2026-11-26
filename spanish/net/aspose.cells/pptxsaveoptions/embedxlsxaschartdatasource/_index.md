---
title: "PptxSaveOptions.EmbedXlsxAsChartDataSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PptxSaveOptions. Indica si se incrusta un archivo xlsx como fuente de datos del gráfico"
type: docs
url: /es/net/aspose.cells/pptxsaveoptions/embedxlsxaschartdatasource/
---
## PptxSaveOptions.EmbedXlsxAsChartDataSource property

Indica si se incrusta un archivo xlsx como fuente de datos del gráfico.

```csharp
public bool EmbedXlsxAsChartDataSource { get; set; }
```

### Observaciones

El valor predeterminado es true.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PptxSaveOptionsPropertyEmbedXlsxAsChartDataSourceDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Crear una hoja de cálculo de ejemplo con datos de gráfico
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);

            // Agregar un gráfico para demostrar el efecto de la propiedad
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";

            try
            {
                // Crear una instancia de PptxSaveOptions
                PptxSaveOptions saveOptions = new PptxSaveOptions();

                // Mostrar el valor predeterminado de EmbedXlsxAsChartDataSource
                Console.WriteLine("Default EmbedXlsxAsChartDataSource value: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Establecer la propiedad a true para demostrar su uso
                saveOptions.EmbedXlsxAsChartDataSource = true;
                Console.WriteLine("EmbedXlsxAsChartDataSource set to: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Guardar el libro de trabajo como PPTX con la opción habilitada
                workbook.Save("EmbedXlsxAsChartDataSourceDemo.pptx", saveOptions);

                Console.WriteLine("PPTX saved with EmbedXlsxAsChartDataSource enabled");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [PptxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


