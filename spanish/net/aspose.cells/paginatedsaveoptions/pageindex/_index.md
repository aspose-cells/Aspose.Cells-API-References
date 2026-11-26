---
title: "PaginatedSaveOptions.PageIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Obtiene o establece el índice basado en 0 de la primera página a guardar"
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/pageindex/
---
## PaginatedSaveOptions.PageIndex property

Obtiene o establece el índice basado en cero de la primera página a guardar.

```csharp
public int PageIndex { get; set; }
```

### Observaciones

El valor predeterminado es 0.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageIndexDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Agregar datos de ejemplo en varias páginas
            for (int i = 0; i < 100; i++)
            {
                sheet.Cells[i, 0].Value = "Data " + (i + 1);
            }

            // Establecer opciones de guardado de PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Configurar para imprimir las páginas 3-4 (índice basado en 0)
            options.PageIndex = 2;  // Third page (index 2)
            options.PageCount = 2; // Print 2 pages
            
            // Guardar el PDF con las páginas seleccionadas
            wb.Save("SelectedPages.pdf", options);
            
            Console.WriteLine("PDF with pages 3-4 created successfully.");
        }
    }
}
```

### Ver también

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


