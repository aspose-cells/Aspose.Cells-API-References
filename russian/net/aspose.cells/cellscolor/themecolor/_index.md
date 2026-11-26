---
title: "CellsColor.ThemeColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство CellsColor. Получает цвет темы. Применяется только для типа цветовой темы"
type: docs
url: /ru/net/aspose.cells/cellscolor/themecolor/
---
## CellsColor.ThemeColor property

Получает цвет темы. Применяется только к типу цвета темы.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellsColorPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Создать экземпляр CellsColor
                CellsColor cellsColor = workbook.CreateCellsColor();

                // Установить цвет темы
                cellsColor.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

                // Отобразить свойства ThemeColor
                Console.WriteLine("ThemeColor Type: " + cellsColor.ThemeColor.ColorType);
                Console.WriteLine("ThemeColor Tint: " + cellsColor.ThemeColor.Tint);

                // Применить цвет к ячейке
                Style style = workbook.CreateStyle();
                style.ForegroundColor = cellsColor.Color;
                style.Pattern = BackgroundType.Solid;

                worksheet.Cells["A1"].PutValue("Theme Color Example");
                worksheet.Cells["A1"].SetStyle(style);

                // Сохраните книгу
                workbook.Save("ThemeColorDemo.xlsx");
                Console.WriteLine("ThemeColor has been demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### См. также

* class [ThemeColor](../../themecolor/)
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


