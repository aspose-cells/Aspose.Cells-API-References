---
title: "PdfBookmarkEntry.Text"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfBookmarkEntry. Título de un marcador"
type: docs
url: /es/net/aspose.cells.rendering/pdfbookmarkentry/text/
---
## PdfBookmarkEntry.Text property

Título de un marcador.

```csharp
public string Text { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfBookmarkEntryPropertyTextDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar contenido de ejemplo
            worksheet.Cells["A1"].PutValue("Page 1 Content");
            
            // Crear entrada de marcador PDF
            PdfBookmarkEntry entry = new PdfBookmarkEntry();
            entry.Text = "Section 1"; // Demonstrating Text property usage
            entry.Destination = worksheet.Cells["A1"];
            entry.IsOpen = true;
            
            // Establecer opciones de guardado con marcador
            PdfSaveOptions saveOptions = new PdfSaveOptions();
            saveOptions.Bookmark = entry;
            
            // Guardar el libro de trabajo con marcador
            workbook.Save("output.pdf", saveOptions);
            
            Console.WriteLine("PDF with bookmark created successfully.");
        }
    }
}
```

### Ver también

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


