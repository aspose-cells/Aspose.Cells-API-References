---
title: "CommentCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método CommentCollection. Elimina el comentario de la celda específica"
type: docs
url: /es/net/aspose.cells/commentcollection/removeat/
---
## RemoveAt(string) {#removeat_2}

Elimina el comentario de la celda específica.

```csharp
public void RemoveAt(string cellName)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellName | String | El nombre de la celda que contiene un comentario. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodRemoveAtWithStringDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar comentarios a celdas usando nombres de celda
            int commentIndex1 = worksheet.Comments.Add("A1");
            worksheet.Comments[commentIndex1].Note = "Comment in A1";
            
            int commentIndex2 = worksheet.Comments.Add("B2");
            worksheet.Comments[commentIndex2].Note = "Comment in B2";
            
            int commentIndex3 = worksheet.Comments.Add("C3");
            worksheet.Comments[commentIndex3].Note = "Comment in C3";
            
            // Eliminar comentario en la celda B2 usando RemoveAt con parámetro de cadena
            worksheet.Comments.RemoveAt("B2");
            
            // Guarda el libro de trabajo
            workbook.Save("CommentsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## RemoveAt(int, int) {#removeat_1}

Elimina el comentario de la celda específica.

```csharp
public void RemoveAt(int row, int column)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| fila | Int32 | El índice de fila. |
| columna | Int32 | el índice de columna. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CommentCollectionMethodRemoveAtWithInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar comentarios a celdas usando referencias de celda
            int comment1Index = worksheet.Comments.Add("A1");
            worksheet.Comments[comment1Index].Note = "First comment";
            
            int comment2Index = worksheet.Comments.Add("B2");
            worksheet.Comments[comment2Index].Note = "Second comment";
            
            int comment3Index = worksheet.Comments.Add("C3");
            worksheet.Comments[comment3Index].Note = "Third comment";
            
            // Eliminar comentario en la fila 1, columna 1 (B2)
            worksheet.Comments.RemoveAt(1, 1);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [CommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


