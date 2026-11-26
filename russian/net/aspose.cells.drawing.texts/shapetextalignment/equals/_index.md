---
title: "ShapeTextAlignment.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод ShapeTextAlignment. Определяет, имеет ли данный экземпляр то же значение, что и другой указанный объект ShapeTextAlignment"
type: docs
url: /ru/net/aspose.cells.drawing.texts/shapetextalignment/equals/
---
## ShapeTextAlignment.Equals method

Определяет, имеет ли данный экземпляр то же значение, что и другой указанный объект [`ShapeTextAlignment`](../).

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Object | Объект [`ShapeTextAlignment`](../) для сравнения с этим экземпляром. |

### Возвращаемое значение

true, если значение параметра obj совпадает со значением данного экземпляра; иначе — false. Если obj равно null, метод возвращает false.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class ShapeTextAlignmentMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавьте фигуру для сравнения выравнивания текста
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;
            
            // Получить выравнивание текста другой фигуры для сравнения
            Shape shape2 = worksheet.Shapes.AddRectangle(2, 0, 1, 0, 100, 100);
            ShapeTextAlignment obj = shape2.TextBody.TextAlignment;

            if (shapeTextAlignment.Equals((object)obj))
            {
                Console.WriteLine("Text alignments are equal");
            }
            else
            {
                Console.WriteLine("Text alignments are not equal");
            }
        }
    }
}
```

### См. также

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


