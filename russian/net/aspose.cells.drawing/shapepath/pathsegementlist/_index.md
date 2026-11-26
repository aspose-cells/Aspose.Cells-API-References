---
title: "ShapePath.PathSegementList"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapePath. Возвращает список ShapeSegmentPathCollection"
type: docs
url: /ru/net/aspose.cells.drawing/shapepath/pathsegementlist/
---
## ShapePath.PathSegementList property

Возвращает список [`ShapeSegmentPathCollection`](../../shapesegmentpathcollection/)

```csharp
[Obsolete("Use ShapePath.PathSegments property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public ShapeSegmentPathCollection PathSegementList { get; }
```

### Примечания

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте свойство ShapePath.PathSegments. Это свойство будет удалено через 12 месяцев, начиная с июля 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyPathSegementListDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //Создать новый путь формы
                ShapePath shapePath = new ShapePath();

                // Перейти к начальной точке
                shapePath.MoveTo(10, 10);

                // Вызвать метод LineTo с параметрами (Single, Single)
                shapePath.LineTo(50.5f, 10.5f);
                shapePath.LineTo(50.5f, 50.5f);
                shapePath.LineTo(10.5f, 50.5f);
                shapePath.Close();

                // Получить доступ к свойству PathSegementList
                ShapeSegmentPathCollection segmentList = shapePath.PathSegementList;

                // Отобразить количество сегментов пути
                Console.WriteLine("Number of path segments: " + segmentList.Count);

                // Итерировать каждый сегмент и отобразить его тип
                foreach (ShapeSegmentPath segment in segmentList)
                {
                    Console.WriteLine("Segment type: " + segment.Type);
                }

                //добавить свободную форму
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("MoveTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }

            // Сохраните книгу
            workbook.Save("ShapePathPropertyPathSegementListDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapeSegmentPathCollection](../../shapesegmentpathcollection/)
* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


