---
title: "LineFormat.Equals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод LineFormat. Определяет, имеет ли данный экземпляр то же значение, что и другой указанный объект LineFormat"
type: docs
url: /ru/net/aspose.cells.drawing/lineformat/equals/
---
## LineFormat.Equals method

Определяет, имеет ли данный экземпляр то же значение, что и другой указанный объект [`LineFormat`](../).

```csharp
public override bool Equals(object obj)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| obj | Object | Объект [`LineFormat`](../), с которым сравнивается данный экземпляр. |

### Возвращаемое значение

true, если значение параметра obj совпадает со значением данного экземпляра; иначе — false. Если obj равно null, метод возвращает false.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatMethodEqualsWithObjectDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Добавить линейную форму на лист
            worksheet.Shapes.AddLine(1, 1, 10, 10, 100, 0);
            
            // Получить формат линии первой фигуры
            LineFormat lineFmt1 = worksheet.Shapes[0].Line;
            LineFormat lineFmt2 = worksheet.Shapes[0].Line;
            
            // Сравнить форматы линий, используя метод Equals
            if (lineFmt1.Equals((object)lineFmt2))
            {
                Console.WriteLine("The line formats are equal.");
            }
            else
            {
                Console.WriteLine("The line formats are not equal.");
            }
        }
    }
}
```

### См. также

* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


