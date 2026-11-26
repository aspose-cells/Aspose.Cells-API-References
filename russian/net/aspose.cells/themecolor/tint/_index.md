---
title: "ThemeColor.Tint"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThemeColor. Получает и задает значение оттенка"
type: docs
url: /ru/net/aspose.cells/themecolor/tint/
---
## ThemeColor.Tint property

Получает и задает значение оттенка.

```csharp
public double Tint { get; set; }
```

### Примечания

Значение оттенка хранится как double от -1.0 до 1.0, где -1.0 означает 100% затемнение, а 1.0 означает 100% осветление. Также 0.0 означает отсутствие изменений.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThemeColorPropertyTintDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создайте стиль с тематическим цветом и оттенком
            Style style = workbook.CreateStyle();
            style.BackgroundThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5); // 0.5 tint
            
            // Применить стиль к ячейке
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);

            // Получите значение оттенка из стиля ячейки
            double tintValue = cell.GetStyle().BackgroundThemeColor.Tint;
            Console.WriteLine("Tint value: " + tintValue);

            // Измените значение оттенка
            ThemeColor themeColor = cell.GetStyle().BackgroundThemeColor;
            themeColor.Tint = 0.8; // Change tint to 0.8
            cell.SetStyle(style);

            // Проверьте новое значение оттенка
            Console.WriteLine("Modified tint value: " + cell.GetStyle().BackgroundThemeColor.Tint);
        }
    }
}
```

### См. также

* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


