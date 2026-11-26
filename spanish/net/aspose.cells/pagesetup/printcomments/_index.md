---
title: "PageSetup.PrintComments"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PageSetup. Representa la forma en que los comentarios se imprimen con la hoja"
type: docs
url: /es/net/aspose.cells/pagesetup/printcomments/
---
## PageSetup.PrintComments property

Representa la forma en que los comentarios se imprimen con la hoja.

```csharp
public PrintCommentsType PrintComments { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintCommentsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar un comentario a la celda A1
            int commentIndex = sheet.Comments.Add("A1");
            Comment comment = sheet.Comments[commentIndex];
            comment.Note = "This is a test comment";

            // Establece diferentes opciones de impresión de comentarios y demuestra sus efectos
            sheet.PageSetup.PrintComments = PrintCommentsType.PrintInPlace;
            Console.WriteLine("PrintComments set to PrintInPlace");

            sheet.PageSetup.PrintComments = PrintCommentsType.PrintSheetEnd;
            Console.WriteLine("PrintComments set to PrintSheetEnd");

            sheet.PageSetup.PrintComments = PrintCommentsType.PrintNoComments;
            Console.WriteLine("PrintComments set to PrintNoComments");

            // Guarda el libro de trabajo para demostrar que la configuración persiste
            workbook.Save("PrintCommentsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* enum [PrintCommentsType](../../printcommentstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


