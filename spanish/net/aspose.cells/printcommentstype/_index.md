---
title: "Enumeración PrintCommentsType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.PrintCommentsType enumeración. Representa la forma en que los comentarios se imprimen con la hoja"
type: docs
url: /es/net/aspose.cells/printcommentstype/
---
## PrintCommentsType enumeration

Representa la forma en que los comentarios se imprimen con la hoja.

```csharp
public enum PrintCommentsType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| PrintInPlace | `0` | Representa imprimir los comentarios tal como se muestran en la hoja. |
| PrintNoComments | `1` | Representa no imprimir los comentarios. |
| PrintSheetEnd | `2` | Representa imprimir los comentarios al final de la hoja. |
| PrintWithThreadedComments | `3` | Representa imprimir los comentarios tal como se muestran en la hoja, incluyendo los comentarios en hilo. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class PrintCommentsTypeDemo
    {
        public static void PrintCommentsTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos comentarios a la hoja de cálculo
            int commentIndex = worksheet.Comments.Add("A1");
            Comment comment = worksheet.Comments[commentIndex];
            comment.Note = "This is a comment.";

            commentIndex = worksheet.Comments.Add("B2");
            comment = worksheet.Comments[commentIndex];
            comment.Note = "This is another comment.";

            // Establecer el tipo de impresión de comentarios en la configuración de página
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.PrintComments = PrintCommentsType.PrintSheetEnd;

            // Guardar el libro de trabajo en un archivo
            workbook.Save("PrintCommentsTypeExample.xlsx");

            Console.WriteLine("Workbook saved successfully with comments printed at the end of the sheet.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


