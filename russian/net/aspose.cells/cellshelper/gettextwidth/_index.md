---
title: "CellsHelper.GetTextWidth"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод CellsHelper. Получить ширину текста в единицах пунктов"
type: docs
url: /ru/net/aspose.cells/cellshelper/gettextwidth/
---
## CellsHelper.GetTextWidth method

Получить ширину текста в единицах точек.

```csharp
public static double GetTextWidth(string text, Font font, double scaling)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| текст | String | Текст. |
| шрифт | Шрифт | Шрифт текста. |
| масштабирование | Double | Масштабирование текста. |

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsHelperMethodGetTextWidthWithStringFontDoubleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Font font = workbook.DefaultStyle.Font;
            double textWidth = CellsHelper.GetTextWidth("Sample Text", font, 1.0);
            Console.WriteLine("Text width: " + textWidth);
        }
    }
}
```

### См. также

* class [Font](../../font/)
* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


