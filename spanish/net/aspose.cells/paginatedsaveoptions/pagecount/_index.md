---
title: "PaginatedSaveOptions.PageCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Obtiene o establece el número de páginas a guardar"
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/pagecount/
---
## PaginatedSaveOptions.PageCount property

Obtiene o establece el número de páginas a guardar.

```csharp
public int PageCount { get; set; }
```

### Observaciones

El valor predeterminado es System.Int32.MaxValue, lo que significa que se renderizarán todas las páginas..

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyPageCountDemo
    {
        public static void Run()
        {
            // Abre un archivo de Excel
            Workbook wb = new Workbook("Book1.xlsx");
            
            // Inicializar opciones de guardado PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Configurar para imprimir solo 2 páginas a partir de la página 4 (índice basado en 0 es 3)
            options.PageIndex = 3;
            options.PageCount = 2;
            
            // Guardar el archivo PDF
            wb.Save("output.pdf", options);
            
            Console.WriteLine("PDF saved with selected pages.");
        }
    }
}
```

### Ver también

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


