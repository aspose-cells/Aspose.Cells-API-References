---
title: "CommentCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CommentCollection. Añade un comentario a la colección"
type: docs
url: /es/net/aspose.cells/commentcollection/add/
---
## Add(int, int) {#add}

Agrega un comentario a la colección.

```csharp
public int Add(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | Índice de fila de la celda. |
| columna | Int32 | Índice de columna de la celda. |

### Valor de retorno

[`Comment`](../../comment/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            CommentCollection comments = worksheet.Comments;
            
            int commentIndex1 = comments.Add(0, 0);
            Comment comment1 = comments[commentIndex1];
            comment1.Note = "First note.";
            comment1.Font.Name = "Times New Roman";
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(string) {#add_1}

Agrega un comentario a la colección.

```csharp
public int Add(string cellName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | String | Nombre de la celda. |

### Valor de retorno

[`Comment`](../../comment/) object index.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodAddWithStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            CommentCollection comments = worksheet.Comments;
            
            int commentIndex1 = comments.Add("A1");
            Comment comment1 = comments[commentIndex1];
            comment1.Note = "First note.";
            comment1.Font.Name = "Arial";
            
            int commentIndex2 = comments.Add("B2");
            Comment comment2 = comments[commentIndex2];
            comment2.Note = "Second note.";
            comment2.Font.Name = "Times New Roman";
            
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


