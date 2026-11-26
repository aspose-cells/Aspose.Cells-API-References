---
title: "Worksheet.Comments"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Worksheet. Obtiene la colección Comment"
type: docs
url: /es/net/aspose.cells/worksheet/comments/
---
## Worksheet.Comments property

Obtiene la colección [`Comment`](../../comment/).

```csharp
public CommentCollection Comments { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyCommentsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue comentarios a las celdas
            worksheet.Cells["A1"].PutValue("Cell A1");
            int commentIndexA1 = worksheet.Comments.Add("A1");
            worksheet.Comments[commentIndexA1].Note = "Note for A1";

            worksheet.Cells["B1"].PutValue("Cell B1");
            int commentIndexB1 = worksheet.Comments.Add("B1");
            worksheet.Comments[commentIndexB1].Note = "Note for B1";

            worksheet.Cells["C2"].PutValue("Cell C2");
            int commentIndexC2 = worksheet.Comments.Add("C2");
            worksheet.Comments[commentIndexC2].Note = "Note for C2";

            // Guarda el libro de trabajo
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CommentCollection](../../commentcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


