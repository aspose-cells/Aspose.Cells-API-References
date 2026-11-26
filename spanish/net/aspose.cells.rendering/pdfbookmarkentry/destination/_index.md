---
title: "PdfBookmarkEntry.Destination"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PdfBookmarkEntry. La celda a la que apunta el enlace del marcador"
type: docs
url: /es/net/aspose.cells.rendering/pdfbookmarkentry/destination/
---
## PdfBookmarkEntry.Destination property

La celda a la que enlaza el marcador.

```csharp
public Cell Destination { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PdfBookmarkEntryPropertyDestinationDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar contenido de ejemplo
            worksheet.Cells["A1"].PutValue("Bookmark Destination");
            
            // Configurar opciones de guardado PDF con marcador
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            PdfBookmarkEntry entry = new PdfBookmarkEntry();
            entry.Text = "Sample Bookmark";
            entry.Destination = worksheet.Cells["A1"]; // Demonstrate Destination property
            entry.IsOpen = true;
            
            pdfSaveOptions.Bookmark = entry;
            
            // Guardar el PDF
            workbook.Save("PdfBookmarkEntryPropertyDestinationDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Ver también

* class [Cell](../../../aspose.cells/cell/)
* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


