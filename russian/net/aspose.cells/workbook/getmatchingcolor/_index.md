---
title: "Workbook.GetMatchingColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Находит наиболее подходящий цвет в текущей палитре"
type: docs
url: /ru/net/aspose.cells/workbook/getmatchingcolor/
---
## Workbook.GetMatchingColor method

Находит наиболее подходящий цвет в текущей палитре.

```csharp
public Color GetMatchingColor(Color rawColor)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| rawColor | Color | Исходный цвет. |

### Возвращаемое значение

Наиболее подходящий цвет.

### Примечания

В палитре цветов Excel 97-2003 всего 56 цветов. Если цвет отсутствует в палитре, будет установлен похожий цвет.

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetMatchingColorWithColorDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            
            // Проверить, существует ли цвет в палитре
            Console.WriteLine("Is Red in palette: " + workbook.IsColorInPalette(Color.Red));
            Color testColor = Color.FromArgb(255, 123, 123, 123);
            Console.WriteLine("Is custom color in palette: " + workbook.IsColorInPalette(testColor));

            // Получить соответствующий цвет из палитры
            Color matchedColor = workbook.GetMatchingColor(testColor);
            Console.WriteLine($"Original color: R={testColor.R}, G={testColor.G}, B={testColor.B}");
            Console.WriteLine($"Matched color: R={matchedColor.R}, G={matchedColor.G}, B={matchedColor.B}");

            // Создать пользовательскую тему
            Color[] themeColors = new Color[12];
            for (int i = 0; i < themeColors.Length; i++)
            {
                themeColors[i] = Color.FromArgb(255, 128 + i, 128 + i, 128 + i);
            }
            workbook.CustomTheme("CustomTheme", themeColors);

            // Получить цвет темы
            Color themeColor = workbook.GetThemeColor(ThemeColorType.FollowedHyperlink);
            Console.WriteLine($"Theme color: R={themeColor.R}, G={themeColor.G}, B={themeColor.B}");
        }
    }
}
```

### См. также

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


