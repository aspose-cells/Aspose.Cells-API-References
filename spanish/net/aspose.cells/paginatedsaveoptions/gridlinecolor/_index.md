---
title: "PaginatedSaveOptions.GridlineColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PaginatedSaveOptions. Obtiene o establece el color de la línea de cuadrícula"
type: docs
url: /es/net/aspose.cells/paginatedsaveoptions/gridlinecolor/
---
## PaginatedSaveOptions.GridlineColor property

Obtiene o establece el color de la línea de cuadrícula.

```csharp
public Color GridlineColor { get; set; }
```

### Observaciones

Ignorará la configuración del color de la línea de cuadrícula en el archivo fuente.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class PaginatedSaveOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].Value = "Gridline Color Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // Crea opciones de guardado PDF
                PdfSaveOptions options = new PdfSaveOptions();

                // Mostrar el valor predeterminado de GridlineColor
                Console.WriteLine("Default GridlineColor: " + options.GridlineColor);

                // Establecer un nuevo color de línea de cuadrícula
                options.GridlineColor = Color.Red;

                // Mostrar el valor actualizado de GridlineColor
                Console.WriteLine("Updated GridlineColor: " + options.GridlineColor);

                // Guardar el libro de trabajo con la configuración del color de la línea de cuadrícula
                workbook.Save("GridlineColorDemo.pdf", options);

                Console.WriteLine("PDF saved with custom gridline color.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


