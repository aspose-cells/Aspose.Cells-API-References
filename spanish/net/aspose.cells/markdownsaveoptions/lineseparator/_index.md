---
title: "MarkdownSaveOptions.LineSeparator"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MarkdownSaveOptions. Obtiene y establece el separador de línea"
type: docs
url: /es/net/aspose.cells/markdownsaveoptions/lineseparator/
---
## MarkdownSaveOptions.LineSeparator property

Obtiene y establece el separador de línea.

```csharp
public string LineSeparator { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertyLineSeparatorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Value1");
            worksheet.Cells["B2"].PutValue("Value2");

            // Configurar opciones de guardado de Markdown con separador de línea personalizado
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                LineSeparator = "\n", // Using Unix-style line endings
                Encoding = Encoding.UTF8
            };

            // Guardar como archivo Markdown
            workbook.Save("MarkdownWithLineSeparator.md", saveOptions);

            Console.WriteLine("Markdown file saved with custom line separator.");
        }
    }
}
```

### Ver también

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


