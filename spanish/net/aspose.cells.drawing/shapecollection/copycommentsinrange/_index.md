---
title: "ShapeCollection.CopyCommentsInRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Copiar todos los comentarios en el rango"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/copycommentsinrange/
---
## ShapeCollection.CopyCommentsInRange method

Copia todos los comentarios en el rango.

```csharp
public void CopyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| formas | ShapeCollection | Las formas de origen. |
| ca | CellArea | El rango de origen. |
| destRow | Int32 | La fila inicial del rango de destino. |
| destColumn | Int32 | La columna inicial del rango de destino. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodCopyCommentsInRangeWithShapeCollectionCellAreaInt32InDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar comentarios
            CommentCollection comments = worksheet.Comments;
            
            // Agregar comentario a la celda A1
            int commentIndex = comments.Add(0, 0);
            Comment comment = comments[commentIndex];
            comment.Note = "First note.";
            comment.Font.Name = "Times New Roman";
            
            // Agregar comentario a la celda B2
            comments.Add("B2");
            comment = comments["B2"];
            comment.Note = "Second note.";
            
            // Definir rango de origen
            CellArea sourceArea = new CellArea();
            sourceArea.StartRow = 0;
            sourceArea.StartColumn = 0;
            sourceArea.EndRow = 1;
            sourceArea.EndColumn = 1;
            
            // Obtener colección de formas
            ShapeCollection shapes = worksheet.Shapes;
            
            // Copiar comentarios del rango de origen al destino (comenzando en la fila 5, columna 1)
            shapes.CopyCommentsInRange(shapes, sourceArea, 5, 1);
            
            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


