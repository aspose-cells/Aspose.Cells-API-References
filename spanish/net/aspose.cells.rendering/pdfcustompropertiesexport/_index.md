---
title: "Enum PdfCustomPropertiesExport"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Rendering.PdfCustomPropertiesExport. Especifica la forma en que CustomDocumentPropertyCollection se exporta al archivo PDF."
type: docs
url: /es/net/aspose.cells.rendering/pdfcustompropertiesexport/
---
## PdfCustomPropertiesExport enumeration

Especifica la forma en que [`CustomDocumentPropertyCollection`](../../aspose.cells.properties/customdocumentpropertycollection/) se exporta al archivo PDF.

```csharp
public enum PdfCustomPropertiesExport
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | No se exportan propiedades personalizadas. |
| Standard | `1` | Las propiedades personalizadas se exportan como entradas en el diccionario Info. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfCustomPropertiesExportDemo
    {
        public static void PdfCustomPropertiesExportExample()
        {
            // Crea un libro de trabajo y agrega algunos datos
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Hello Aspose");
            worksheet.Cells["A2"].PutValue("This is a sample document");

            // Establece algunas propiedades personalizadas
            workbook.Worksheets.CustomDocumentProperties.Add("Author", "John Doe");
            workbook.Worksheets.CustomDocumentProperties.Add("Subject", "Sample PDF Export");

            // Crea opciones de guardado PDF
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            
            // Establece la opción de exportación de propiedades personalizadas
            saveOptions.CustomPropertiesExport = PdfCustomPropertiesExport.Standard;

            // Guarda el libro de trabajo en PDF
            workbook.Save("PdfCustomPropertiesExportExample.pdf", saveOptions);

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


