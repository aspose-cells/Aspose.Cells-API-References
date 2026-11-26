---
title: "MarkdownSaveOptions.TableHeaderType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MarkdownSaveOptions. Obtiene y establece cómo se define el encabezado de la tabla"
type: docs
url: /es/net/aspose.cells/markdownsaveoptions/tableheadertype/
---
## MarkdownSaveOptions.TableHeaderType property

Obtiene y establece cómo definir el encabezado de la tabla.

```csharp
public MarkdownTableHeaderType TableHeaderType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Markdown;

namespace AsposeCellsExamples
{
    public class MarkdownSaveOptionsPropertyTableHeaderTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para crear una tabla
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // Crear MarkdownSaveOptions y establecer TableHeaderType
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;

            // Guardar como markdown con opciones especificadas
            workbook.Save("output.md", saveOptions);
        }
    }
}
```

### Ver también

* enum [MarkdownTableHeaderType](../../../aspose.cells.markdown/markdowntableheadertype/)
* class [MarkdownSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


