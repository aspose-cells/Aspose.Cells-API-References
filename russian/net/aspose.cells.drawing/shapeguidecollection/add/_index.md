---
title: "ShapeGuideCollection.Add"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeGuideCollection. Добавляет направляющую формы. Важно: эта функция в настоящее время доступна только для Excel07 и выше"
type: docs
url: /ru/net/aspose.cells.drawing/shapeguidecollection/add/
---
## ShapeGuideCollection.Add method

Добавляет направляющую формы.(Важно: Эта функция в настоящее время доступна только для Excel07 и выше)

```csharp
public int Add(string name, double val)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| name | String | имя корректировки. Оно выглядит как "adj(Используется, когда есть только одно значение корректировки)", "adj1", "adj2", "adj3" и т.д. |
| val | Double | значение корректировки |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuideCollectionMethodAddWithStringDoubleDemo
    {
        public static void Run()
        {
            // Создайте новую книгу и получите доступ к первому листу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму, использующую направляющие корректировки
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 2, 0, 2, 0, 200, 150);

            try
            {
                // Получить ShapeGuideCollection из корректировок геометрии формы
                ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;

                // Вызвать метод Add с параметрами (String, Double)
                shapeGuides.Add("adj1", 25.5);
                shapeGuides.Add("adj2", 25.5);
                shapeGuides.Add("adj3", 25.5);
                shapeGuides.Add("adj4", 25.5);

                Console.WriteLine($"Total guides after addition: {shapeGuides.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Сохранить изменённую книгу
            workbook.Save("ShapeGuideAddWithStringDoubleDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapeGuideCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


