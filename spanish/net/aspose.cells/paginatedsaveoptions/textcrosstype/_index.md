---
title: "PaginatedSaveOptions.TextCrossType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Obtiene o establece el tipo de visualización de texto cuando el ancho del texto es mayor que el ancho de la celda"
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/textcrosstype/
---
## PaginatedSaveOptions.TextCrossType property

Obtiene o establece el tipo de visualización de texto cuando el ancho del texto es mayor que el ancho de la celda.

```csharp
public TextCrossType TextCrossType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyTextCrossTypeDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Establecer texto largo que cruzará los límites de la celda
            worksheet.Cells["A1"].PutValue("This is a long text that will cross cell boundaries");
            worksheet.Cells["B1"].PutValue("Another cell content");
            
            // Establecer el ancho de columna para que el texto cruce celdas
            worksheet.Cells.SetColumnWidth(0, 5);
            
            // Crea opciones de guardado PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Demostrar TextCrossType configurándolo a CrossKeep
            options.TextCrossType = TextCrossType.CrossKeep;
            
            // Guardar el libro de trabajo como PDF
            workbook.Save("TextCrossTypeDemo.pdf", options);
            
            Console.WriteLine("PDF saved with TextCrossType.CrossKeep setting");
        }
    }
}
```

### Ver también

* enum [TextCrossType](../../textcrosstype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


