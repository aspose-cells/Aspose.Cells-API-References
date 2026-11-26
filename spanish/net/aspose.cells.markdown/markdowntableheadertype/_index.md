---
title: "Enum MarkdownTableHeaderType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Markdown.MarkdownTableHeaderType. Representa el tipo de encabezado de la tabla en el archivo markdown"
type: docs
url: /es/net/aspose.cells.markdown/markdowntableheadertype/
---
## MarkdownTableHeaderType enumeration

Representa el tipo de encabezado de la tabla en el archivo markdown.

```csharp
public enum MarkdownTableHeaderType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| FirstRow | `0` | Primera fila como encabezado de la tabla. |
| ColumnHeader | `1` | Nombre de columna (como A,B,C...) como encabezado de la tabla. |
| Empty | `2` | Una fila de encabezado vacía. |

### Ejemplos

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Markdown;

namespace AsposeCellsExamples
{
    public class MarkdownClassMarkdownTableHeaderTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue("Data2");

            // Establecer opciones de guardado de Markdown
            MarkdownSaveOptions saveOptions = new MarkdownSaveOptions();
            saveOptions.TableHeaderType = MarkdownTableHeaderType.FirstRow;
            
            // Guardar como archivo Markdown
            workbook.Save("output.md", saveOptions);
            
            // Verificar la salida
            string text = File.ReadAllText("output.md");
            Console.WriteLine(text.Contains("---|") ? "Success" : "Failed");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Markdown](../../aspose.cells.markdown/)
* assembly [Aspose.Cells](../../)


