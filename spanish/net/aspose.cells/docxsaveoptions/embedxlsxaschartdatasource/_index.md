---
title: "DocxSaveOptions.EmbedXlsxAsChartDataSource"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DocxSaveOptions. Indica si se incrusta un archivo xlsx como fuente de datos del gráfico"
type: docs
url: /es/net/aspose.cells/docxsaveoptions/embedxlsxaschartdatasource/
---
## DocxSaveOptions.EmbedXlsxAsChartDataSource property

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
    using System;

    public class DocxSaveOptionsPropertyEmbedXlsxAsChartDataSourceDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceda a la primera hoja de cálculo y agregue datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Chart Data";

            try
            {
                // Inicialice DocxSaveOptions
                DocxSaveOptions saveOptions = new DocxSaveOptions();

                // Mostrar el valor predeterminado de la propiedad EmbedXlsxAsChartDataSource
                Console.WriteLine("Default EmbedXlsxAsChartDataSource value: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Establecer EmbedXlsxAsChartDataSource a true para demostrar su uso
                saveOptions.EmbedXlsxAsChartDataSource = true;
                Console.WriteLine("EmbedXlsxAsChartDataSource set to: " + saveOptions.EmbedXlsxAsChartDataSource);

                // Guarde el libro de trabajo como DOCX con las opciones configuradas
                workbook.Save("EmbedXlsxAsChartDataSourceDemo.docx", saveOptions);
                Console.WriteLine("Document saved successfully with EmbedXlsxAsChartDataSource option.");
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

* class [DocxSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


