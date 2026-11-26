---
title: "HtmlSaveOptions.ExportDocumentProperties"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad HtmlSaveOptions. Indica si se exportan las propiedades del documento. El valor predeterminado es verdadero. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado"
type: docs
url: /es/net/aspose.cells/htmlsaveoptions/exportdocumentproperties/
---
## HtmlSaveOptions.ExportDocumentProperties property

Indica si se exportan las propiedades del documento. El valor predeterminado es true. Si desea importar el archivo html o mht a Excel, mantenga el valor predeterminado.

```csharp
public bool ExportDocumentProperties { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportDocumentPropertiesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunas propiedades del documento
            workbook.BuiltInDocumentProperties.Author = "Test Author";
            workbook.BuiltInDocumentProperties.Title = "Test Document";
            
            // Agregar datos de celda de ejemplo
            worksheet.Cells["A1"].PutValue("Sample HTML Export");
            
            // Crear opciones de guardado HTML y establecer ExportDocumentProperties en falso
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportDocumentProperties = false;
            
            // Guarda el libro de trabajo como HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with document properties export disabled.");
        }
    }
}
```

### Ver también

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


