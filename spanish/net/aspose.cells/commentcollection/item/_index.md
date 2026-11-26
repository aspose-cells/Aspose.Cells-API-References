---
title: "CommentCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CommentCollection. Obtiene el elemento Comment en el índice especificado"
type: docs
url: /es/net/aspose.cells/commentcollection/item/
---
## CommentCollection indexer (1 of 3)

Obtiene el elemento [`Comment`](../../comment/) en el índice especificado.

```csharp
public Comment this[int index] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| índice | El índice basado en cero del elemento. |

### Valor de retorno

El elemento en el índice especificado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo1
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue comentarios a las celdas
            int commentIndex1 = worksheet.Comments.Add("A1");
            int commentIndex2 = worksheet.Comments.Add("B2");
            
            // Acceder a los comentarios usando la propiedad Item
            Comment comment1 = worksheet.Comments[commentIndex1];
            Comment comment2 = worksheet.Comments[commentIndex2];
            
            // Establecer notas del comentario
            comment1.Note = "First comment";
            comment2.Note = "Second comment";
            
            // Modificar el primer comentario usando la propiedad Item
            worksheet.Comments[0].Note = "Updated first comment";
            
            // Acceder y modificar el comentario directamente desde la colección
            Comment comment3 = worksheet.Comments[1];
            comment3.Note = "Updated second comment";
            
            // Guarda el libro de trabajo
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CommentCollection indexer (2 of 3)

Obtiene el elemento [`Comment`](../../comment/) en la celda especificada.

```csharp
public Comment this[string cellName] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| cellName | Nombre de la celda. |

### Valor de retorno

El elemento en la celda especificada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo2
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar comentarios a celdas usando referencias de celda
            int comment1Index = worksheet.Comments.Add(0, 0); // A1
            worksheet.Comments[comment1Index].Note = "First comment";
            
            int comment2Index = worksheet.Comments.Add(1, 1); // B2
            worksheet.Comments[comment2Index].Note = "Second comment";
            
            int comment3Index = worksheet.Comments.Add(2, 2); // C3
            worksheet.Comments[comment3Index].Note = "Third comment";

            // Acceder a los comentarios usando la propiedad Item con referencias de celda
            CommentCollection comments = worksheet.Comments;
            Comment comment1 = comments["A1"];
            Comment comment2 = comments["B2"];
            Comment comment3 = comments["C3"];

            // Modificar notas de los comentarios
            comment1.Note = "Updated first note";
            comment2.Note = "Updated second note";
            comment3.Note = "Updated third note";

            // Guarda el libro de trabajo
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CommentCollection indexer (3 of 3)

Obtiene el elemento [`Comment`](../../comment/) en el índice de fila y columna especificados.

```csharp
public Comment this[int row, int column] { get; }
```

| Parámetro | Descripción |
| --- | --- |
| fila | Índice de fila. |
| columna | Índice de columna. |

### Valor de retorno

El elemento en la celda especificada.

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar comentarios a celdas usando referencias de celda
            int comment1Index = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1Index].Note = "First comment";

            int comment2Index = worksheet.Comments.Add("B2");
            worksheet.Comments[comment2Index].Note = "Second comment";

            int comment3Index = worksheet.Comments.Add("C3");
            worksheet.Comments[comment3Index].Note = "Third comment";

            // Acceder a los comentarios usando la propiedad Item con índices de fila/columna
            CommentCollection comments = worksheet.Comments;
            Comment comment1 = comments[0, 0];
            comment1.Note = "Updated first comment";

            Comment comment2 = comments[1, 1];
            comment2.Note = "Updated second comment";

            // Guarda el libro de trabajo
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Comment](../../comment/)
* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


