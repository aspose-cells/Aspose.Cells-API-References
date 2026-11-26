---
title: "MarkdownSaveOptions.Encoding"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MarkdownSaveOptions. Obtiene y establece la codificación predeterminada"
type: docs
url: /es/net/aspose.cells/markdownsaveoptions/encoding/
---
## MarkdownSaveOptions.Encoding property

Obtiene y establece la codificación predeterminada.

```csharp
public Encoding Encoding { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertyEncodingDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Sample");
            worksheet.Cells["B1"].PutValue("Markdown");

            // Configurar opciones de guardado con codificación UTF8
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions
            {
                Encoding = Encoding.UTF8
            };

            // Guardar con codificación especificada
            workbook.Save("MarkdownWithEncoding.md", saveOptions);

            Console.WriteLine("Markdown file saved with UTF-8 encoding.");
        }
    }
}
```

### Ver también

* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


