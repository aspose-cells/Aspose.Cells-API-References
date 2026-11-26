---
title: "Border.ThemeColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Border. Получает и задает цвет темы границы"
type: docs
url: /ru/net/aspose.cells/border/themecolor/
---
## Border.ThemeColor property

Получает и задаёт цвет темы границы.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Обратиться к ячейке и получить её стиль
            Style style = worksheet.Cells["A1"].GetStyle();

            // Установить цвет темы границы
            style.Borders[BorderType.BottomBorder].ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            // Применить стиль к ячейке
            worksheet.Cells["A1"].SetStyle(style);

            // Сохраните книгу
            workbook.Save("BorderThemeColorDemo.xlsx");
        }
    }
}
```

### См. также

* class [ThemeColor](../../themecolor/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


