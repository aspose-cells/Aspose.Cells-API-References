---
title: "PaginatedSaveOptions.GridlineType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Obtiene o establece el tipo de línea de cuadrícula"
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/gridlinetype/
---
## PaginatedSaveOptions.GridlineType property

Obtiene o establece el tipo de línea de cuadrícula.

```csharp
public GridlineType GridlineType { get; set; }
```

### Observaciones

El valor predeterminado es tipo Dotted.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyGridlineTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo y habilitar líneas de cuadrícula
            worksheet.Cells["A1"].PutValue("GridlineType Demo");
            worksheet.Cells["B2"].PutValue(1);
            worksheet.Cells["C3"].PutValue(2);
            worksheet.Cells["D4"].PutValue(3);
            worksheet.IsGridlinesVisible = true;

            // Crea opciones de guardado PDF
            PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
            
            // Demostrar la propiedad GridlineType
            pdfSaveOptions.GridlineType = GridlineType.Dotted;

            // Guardar el libro de trabajo con líneas de cuadrícula
            workbook.Save("GridlineTypeDemo.pdf", pdfSaveOptions);
        }
    }
}
```

### Ver también

* enum [GridlineType](../../gridlinetype/)
* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


