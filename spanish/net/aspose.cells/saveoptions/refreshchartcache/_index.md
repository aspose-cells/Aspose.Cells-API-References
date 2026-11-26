---
title: "SaveOptions.RefreshChartCache"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SaveOptions. Indica si se debe almacenar en caché los datos más recientes del gráfico"
type: docs
url: /es/net/aspose.cells/saveoptions/refreshchartcache/
---
## SaveOptions.RefreshChartCache property

Indica si se almacena en caché los datos más recientes del gráfico.

```csharp
public bool RefreshChartCache { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SaveOptionsPropertyRefreshChartCacheDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo de ejemplo con un gráfico
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Crear opciones de guardado PDF con RefreshChartCache habilitado
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            pdfSaveOptions.RefreshChartCache = true;

            // Guardar el libro de trabajo con la opción de refrescar la caché del gráfico
            workbook.Save("output.pdf", pdfSaveOptions);

            Console.WriteLine("Workbook saved with chart cache refreshed.");
        }
    }
}
```

### Ver también

* class [SaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


