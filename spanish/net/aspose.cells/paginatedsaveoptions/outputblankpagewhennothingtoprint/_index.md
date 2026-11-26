---
title: "PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Indica si se debe generar una página en blanco cuando no hay nada que imprimir"
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/
---
## PaginatedSaveOptions.OutputBlankPageWhenNothingToPrint property

Indica si se debe generar una página en blanco cuando no hay nada que imprimir.

```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```

### Observaciones

El valor predeterminado es true.

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaginatedSaveOptionsPropertyOutputBlankPageWhenNothingToPrintDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo y ocultarla (simulando que no hay nada que imprimir)
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.IsVisible = false;

            // Establecer opciones de guardado de PDF con OutputBlankPageWhenNothingToPrint = false
            PdfSaveOptions options = new PdfSaveOptions
            {
                OutputBlankPageWhenNothingToPrint = false
            };

            // Guardar en PDF - no se debe generar una página en blanco
            string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputNoBlankPage.pdf");
            workbook.Save(outputPath, options);

            // Cambiar la opción a true
            options.OutputBlankPageWhenNothingToPrint = true;

            // Guardar de nuevo - se debe generar una página en blanco
            outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "OutputWithBlankPage.pdf");
            workbook.Save(outputPath, options);
        }
    }
}
```

### Ver también

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


