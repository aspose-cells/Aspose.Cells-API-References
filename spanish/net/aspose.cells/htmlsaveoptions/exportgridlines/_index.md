---
title: "HtmlSaveOptions.ExportGridLines"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exportan las líneas de cuadrícula. El valor predeterminado es false"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportgridlines/
---
## HtmlSaveOptions.ExportGridLines property

Indica si se exportan las líneas de cuadrícula. El valor predeterminado es false.

```csharp
public bool ExportGridLines { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportGridLinesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Establecer la visibilidad de las líneas de cuadrícula
            worksheet.IsGridlinesVisible = true;

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B2"].PutValue(123);
            worksheet.Cells["C3"].PutValue(DateTime.Now);

            // Crear opciones de guardado HTML
            HtmlSaveOptions options = new HtmlSaveOptions
            {
                ExportGridLines = worksheet.IsGridlinesVisible,
                ExportActiveWorksheetOnly = true
            };

            // Guardar como HTML
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with ExportGridLines: " + options.ExportGridLines);
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


