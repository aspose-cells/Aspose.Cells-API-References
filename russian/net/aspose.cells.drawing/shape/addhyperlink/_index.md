---
title: "Shape.AddHyperlink"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Shape. Добавляет гиперссылку к фигуре"
type: docs
url: /ru/net/aspose.cells.drawing/shape/addhyperlink/
---
## Shape.AddHyperlink method

Добавляет гиперссылку к фигуре.

```csharp
public Hyperlink AddHyperlink(string address)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| address | String | Адрес гиперссылки. |

### Возвращаемое значение

Возвращает новый объект гиперссылки.

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodAddHyperlinkWithStringDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Добавить форму на лист
            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 0, 0);

            // Добавьте гиперссылку к фигуре, используя строку URL
            Aspose.Cells.Hyperlink hyperlink = shape.AddHyperlink("https://www.aspose.com/");

            // Сохраните книгу
            workbook.Save("ShapeWithHyperlink.xlsx");
        }
    }
}
```

### См. также

* class [Hyperlink](../../../aspose.cells/hyperlink/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


