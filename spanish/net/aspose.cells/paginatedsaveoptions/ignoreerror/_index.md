---
title: "PaginatedSaveOptions.IgnoreError"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Indica si necesita ocultar el error durante la renderización. El error puede ser un error en la renderización de formas, imágenes, gráficos, etc."
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/ignoreerror/
---
## PaginatedSaveOptions.IgnoreError property

Indica si necesita ocultar el error durante el renderizado. El error puede ser un error en la forma, imagen, renderizado de gráfico, etc.

```csharp
public bool IgnoreError { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyIgnoreErrorDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar algunos datos de ejemplo con posibles errores de formato
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);
            worksheet.Cells["A3"].PutValue(DateTime.Now);
            
            // Crea opciones de guardado PDF
            PdfSaveOptions options = new PdfSaveOptions();
            
            // Establezca IgnoreError en true para omitir cualquier error de conversión
            options.IgnoreError = true;
            
            // Guardar el libro de trabajo como PDF
            workbook.Save("PaginatedSaveWithIgnoreError.pdf", options);
            
            Console.WriteLine("PDF saved with IgnoreError enabled.");
        }
    }
}
```

### Ver también

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


