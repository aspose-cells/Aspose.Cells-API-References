---
title: "MarkdownSaveOptions.FormatStrategy"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MarkdownSaveOptions. Obtiene y establece la estrategia de formato al exportar el valor de la celda como cadena"
type: docs
url: /es/net/aspose.cells/markdownsaveoptions/formatstrategy/
---
## MarkdownSaveOptions.FormatStrategy property

Obtiene y establece la estrategia de formato al exportar el valor de la celda como cadena.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo con diferentes formatos
            worksheet.Cells["A1"].PutValue(123.456); // Numeric value
            worksheet.Cells["A2"].PutValue(DateTime.Now); // Date value
            worksheet.Cells["A3"].PutValue(true); // Boolean value

            // Crear opciones de guardado Markdown con la estrategia de formato DisplayString
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                FormatStrategy = CellValueFormatStrategy.DisplayString
            };

            // Guardar el libro de trabajo como Markdown
            workbook.Save("MarkdownWithDisplayString.md", saveOptions);

            // Cambiar a CellValueFormatStrategy.CellStyle
            saveOptions.FormatStrategy = CellValueFormatStrategy.CellStyle;
            workbook.Save("MarkdownWithCellStyle.md", saveOptions);

            Console.WriteLine("Markdown files saved successfully with different format strategies.");
        }
    }
}
```

### Ver también

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


