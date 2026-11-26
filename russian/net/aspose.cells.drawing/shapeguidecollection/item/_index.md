---
title: "ShapeGuideCollection.Item"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapeGuideCollection. Получает направляющую формы по индексу"
type: docs
url: /ru/net/aspose.cells.drawing/shapeguidecollection/item/
---
## ShapeGuideCollection indexer

Получает направляющую формы по индексу

```csharp
public ShapeGuide this[int index] { get; }
```

| Параметр | Описание |
| --- | --- |
| индекс |  |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuideCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму, использующую направляющие корректировки
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 2, 0, 2, 0, 200, 150);

            // Получить доступ к коллекции направляющих корректировки формы через Geometry
            ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;

            // Добавить новые направляющие в коллекцию
            shapeGuides.Add("adj1", 25.5);
            shapeGuides.Add("adj2", 30);
            shapeGuides.Add("adj3", 25.5);
            shapeGuides.Add("adj4", 35);

            // Продемонстрировать чтение значений направляющих (свойство Name недоступно в предоставленном определении)
            Console.WriteLine("First guide value: " + shapeGuides[0].Value);
            Console.WriteLine("Second guide value: " + shapeGuides[1].Value);
            Console.WriteLine("third guide value: " + shapeGuides[2].Value);
            Console.WriteLine("fourth guide value: " + shapeGuides[3].Value);

            // Сохранить изменённую книгу
            workbook.Save("ShapeGuideCollectionPropertyItemDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapeGuide](../../shapeguide/)
* class [ShapeGuideCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


