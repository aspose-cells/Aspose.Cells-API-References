---
title: "HtmlSaveOptions.ExportPageFooters"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exportan los encabezados de página"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportpagefooters/
---
## HtmlSaveOptions.ExportPageFooters property

Indica si se exportan los encabezados de página.

```csharp
public bool ExportPageFooters { get; set; }
```

### Observaciones

Solo funciona cuando [`SaveAsSingleFile`](../saveassinglefile/) es True.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportPageFootersDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Crear opciones de guardado HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            
            // Establecer ExportPageFooters a true para incluir los pies de página en la salida
            saveOptions.ExportPageFooters = true;
            
            // Establecer otras opciones necesarias
            saveOptions.ExportPageHeaders = true;
            
            // Guardar el libro de trabajo en HTML
            workbook.Save("HtmlWithPageFooters.html", saveOptions);
            
            Console.WriteLine("HTML file with page footers exported successfully.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


