---
title: "HtmlSaveOptions.ExportPageHeaders"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exportan los encabezados de página"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportpageheaders/
---
## HtmlSaveOptions.ExportPageHeaders property

Indica si se exportan los encabezados de página.

```csharp
public bool ExportPageHeaders { get; set; }
```

### Observaciones

Solo funciona cuando [`SaveAsSingleFile`](../saveassinglefile/) es True.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPageHeadersDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer encabezado de página
            worksheet.PageSetup.SetHeader(0, "Sample Header Text");
            
            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("This is a test");
            
            // Configurar opciones de guardado HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                SaveAsSingleFile = true,
                ShowAllSheets = true,
                ExportPageHeaders = true  // This is the key property being demonstrated
            };
            
            // Guarda el libro de trabajo como HTML
            string outputPath = "output_with_headers.html";
            workbook.Save(outputPath, saveOptions);
            
            Console.WriteLine("HTML file with page headers exported successfully.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


