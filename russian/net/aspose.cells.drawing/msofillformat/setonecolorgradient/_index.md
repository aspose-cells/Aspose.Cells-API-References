---
title: "MsoFillFormat.SetOneColorGradient"
second_title: "Справочник API Aspose.Cells для .NET"
description: "MsoFillFormat method. Устанавливает указанную заливку в градиент из одного цвета"
type: docs
url: /ru/net/aspose.cells.drawing/msofillformat/setonecolorgradient/
---
## MsoFillFormat.SetOneColorGradient method

Устанавливает указанное заполнение в градиент из одного цвета.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| цвет | Color | Один цвет градиента. |
| степень | Double | Степень градиента. Может принимать значение от 0.0 (тёмный) до 1.0 (светлый). |
| стиль | GradientStyleType | Стиль затенения градиента. |
| variant | Int32 | Вариант градиента. Может принимать значение от 1 до 4, соответствующее одному из четырёх вариантов на вкладке Gradient в диалоговом окне Fill Effects. Если стиль равен GradientStyle.FromCenter, аргумент Variant может быть только 1 или 2. |

### Примеры

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoFillFormatMethodSetOneColorGradientWithColorDoubleGradientStyleTypeInDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape shape = worksheet.Shapes.AddRectangle(1, 1, 100, 100, 50, 50);
            MsoFillFormat fillFormat = shape.FillFormat;

            // Установить градиент из одного цвета с указанными параметрами
            fillFormat.SetOneColorGradient(Color.Red, 0.5, GradientStyleType.DiagonalUp, 2);

            workbook.Save("GradientFillExample.xlsx");
        }
    }
}
```

### См. также

* enum [GradientStyleType](../../gradientstyletype/)
* class [MsoFillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


