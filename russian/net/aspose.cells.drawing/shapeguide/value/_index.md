---
title: "ShapeGuide.Value"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ShapeGuide. Получает или задает значение этого направляющего"
type: docs
url: /ru/net/aspose.cells.drawing/shapeguide/value/
---
## ShapeGuide.Value property

Получает или задает значение этой направляющей

```csharp
public double Value { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuidePropertyValueDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать форму, использующую направляющие корректировки
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


            Console.WriteLine("Updated adjustment values");

            shapeGuides[0].Value = 25.5;
            shapeGuides[1].Value = 25.5;
            shapeGuides[2].Value = 25.5;
            shapeGuides[3].Value = 25.5;            

            Console.WriteLine("First guide value: " + shapeGuides[0].Value);
            Console.WriteLine("Second guide value: " + shapeGuides[1].Value);
            Console.WriteLine("third guide value: " + shapeGuides[2].Value);
            Console.WriteLine("fourth guide value: " + shapeGuides[3].Value);
            
            // Сохранить изменённую книгу
            workbook.Save("ShapeGuideValueDemo.xlsx");
        }
    }
}
```

### См. также

* class [ShapeGuide](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


