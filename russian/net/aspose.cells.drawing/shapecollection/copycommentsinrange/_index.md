---
title: "ShapeCollection.CopyCommentsInRange"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeCollection. Скопировать все комментарии в диапазоне"
type: docs
url: /ru/net/aspose.cells.drawing/shapecollection/copycommentsinrange/
---
## ShapeCollection.CopyCommentsInRange method

Скопировать все комментарии в диапазоне.

```csharp
public void CopyCommentsInRange(ShapeCollection shapes, CellArea ca, int destRow, int destColumn)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| фигуры | ShapeCollection | Исходные фигуры. |
| ca | CellArea | Исходный диапазон. |
| destRow | Int32 | Начальная строка целевого диапазона. |
| destColumn | Int32 | Начальный столбец целевого диапазона. |

### Примеры

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
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить комментарии
            CommentCollection comments = worksheet.Comments;
            
            // Добавить комментарий в ячейку A1
            int commentIndex = comments.Add(0, 0);
            Comment comment = comments[commentIndex];
            comment.Note = "First note.";
            comment.Font.Name = "Times New Roman";
            
            // Добавить комментарий в ячейку B2
            comments.Add("B2");
            comment = comments["B2"];
            comment.Note = "Second note.";
            
            // Определить исходный диапазон
            CellArea sourceArea = new CellArea();
            sourceArea.StartRow = 0;
            sourceArea.StartColumn = 0;
            sourceArea.EndRow = 1;
            sourceArea.EndColumn = 1;
            
            // Получить коллекцию фигур
            ShapeCollection shapes = worksheet.Shapes;
            
            // Скопировать комментарии из исходного диапазона в целевой (начиная со строки 5, столбца 1)
            shapes.CopyCommentsInRange(shapes, sourceArea, 5, 1);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


