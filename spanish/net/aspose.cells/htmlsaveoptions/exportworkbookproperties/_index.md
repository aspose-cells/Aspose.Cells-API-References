---
title: "HtmlSaveOptions.ExportWorkbookProperties"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exportan las propiedades del libro de trabajo. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado."
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportworkbookproperties/
---
## HtmlSaveOptions.ExportWorkbookProperties property

Indica si se exportan las propiedades del libro de trabajo. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado.

```csharp
public bool ExportWorkbookProperties { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportWorkbookPropertiesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar algunos datos al libro de trabajo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello World!");
            
            // Establecer propiedades del libro de trabajo
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Title";

            // Crear opciones de guardado HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Demostrar ExportWorkbookProperties configurándolo en false
            options.ExportWorkbookProperties = false;
            
            // Guarda el libro de trabajo como HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with ExportWorkbookProperties set to false");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


