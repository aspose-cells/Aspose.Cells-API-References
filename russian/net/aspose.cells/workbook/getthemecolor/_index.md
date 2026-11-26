---
title: "Workbook.GetThemeColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Получает цвет темы"
type: docs
url: /ru/net/aspose.cells/workbook/getthemecolor/
---
## Workbook.GetThemeColor method

Получает цвет темы.

```csharp
public Color GetThemeColor(ThemeColorType type)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | ThemeColorType | Тип цвета темы. |

### Возвращаемое значение

Цвет темы.

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodGetThemeColorWithThemeColorTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить цвет темы для Accent6
            Color color = workbook.GetThemeColor(ThemeColorType.Accent6);
            Console.WriteLine("Theme Color (Accent6): " + color.ToString());
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


