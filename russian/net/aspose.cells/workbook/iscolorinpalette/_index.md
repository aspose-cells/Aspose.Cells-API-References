---
title: "Workbook.IsColorInPalette"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Проверяет, находится ли цвет в палитре таблицы"
type: docs
url: /ru/net/aspose.cells/workbook/iscolorinpalette/
---
## Workbook.IsColorInPalette method

Проверяет, находится ли цвет в палитре электронных таблиц.

```csharp
public bool IsColorInPalette(Color color)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| цвет | Color | Структура Color. |

### Возвращаемое значение

Возвращает true, если этот цвет находится в палитре. В противном случае возвращает false

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodIsColorInPaletteWithColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Проверить, существует ли стандартный цвет в палитре
            bool isRedInPalette = workbook.IsColorInPalette(Color.Red);
            Console.WriteLine("Is Red in palette: " + isRedInPalette);
            
            // Проверить, существует ли пользовательский цвет в палитре
            Color customColor = Color.FromArgb(255, 123, 123, 123);
            bool isCustomInPalette = workbook.IsColorInPalette(customColor);
            Console.WriteLine("Is custom color in palette: " + isCustomInPalette);
            
            // Получить соответствующий цвет из палитры
            Color matchedColor = workbook.GetMatchingColor(customColor);
            Console.WriteLine("Matched color R value: " + matchedColor.R);
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


