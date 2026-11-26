---
title: "Workbook.SetThemeColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Метод Workbook. Устанавливает цвет темы"
type: docs
url: /ru/net/aspose.cells/workbook/setthemecolor/
---
## Workbook.SetThemeColor method

Устанавливает цвет темы

```csharp
public void SetThemeColor(ThemeColorType type, Color color)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | ThemeColorType | Тип цвета темы. |
| цвет | Color | цвет темы |

### Примеры

```csharp
using System;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodSetThemeColorWithThemeColorTypeColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Установить цвет темы для Text1 в зеленый
            workbook.SetThemeColor(ThemeColorType.Text1, Color.Green);
            
            // Применить цвет темы к стилю по умолчанию
            Style style = workbook.DefaultStyle;
            style.Font.ThemeColor = new ThemeColor(ThemeColorType.Text1, 0);
            workbook.DefaultStyle = style;
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
            
            Console.WriteLine("Workbook with theme color saved successfully.");
        }
    }
}
```

### См. также

* enum [ThemeColorType](../../themecolortype/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


