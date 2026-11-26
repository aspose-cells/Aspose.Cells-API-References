---
title: "MarkdownSaveOptions.MarkdownSaveOptions"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor MarkdownSaveOptions. Crea opciones para guardar un documento markdown"
type: docs
url: /es/net/aspose.cells/markdownsaveoptions/markdownsaveoptions/
---
## MarkdownSaveOptions constructor

Crea opciones para guardar el documento markdown

```csharp
public MarkdownSaveOptions()
```

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsMethodCtorDemo
    {
        public static void Run()
        {
            // Crea un nuevo libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);

            // Demostrar el constructor MarkdownSaveOptions
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                Encoding = Encoding.UTF8,
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                LineSeparator = Environment.NewLine
            };

            // Guardar como Markdown
            workbook.Save("MarkdownOutput.md", saveOptions);

            Console.WriteLine("Markdown file created successfully.");
        }
    }
}
```

### Ver también

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


