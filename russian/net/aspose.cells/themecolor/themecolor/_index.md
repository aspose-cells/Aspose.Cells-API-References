---
title: "ThemeColor.ThemeColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Конструктор ThemeColor."
type: docs
url: /ru/net/aspose.cells/themecolor/themecolor/
---
## ThemeColor constructor

```csharp
public ThemeColor(ThemeColorType type, double tint)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| type | ThemeColorType | Тип темы. |
| оттенок | Double | Значение оттенка. |

### Примеры

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThemeColorMethodCtorWithThemeColorTypeDoubleDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Вызовите метод #ctor с параметрами ThemeColorType и Double
                ThemeColor themeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

                // Примените тематический цвет к стилю ячейки
                Style style = workbook.CreateStyle();
                style.ForegroundThemeColor = themeColor;
                style.Pattern = BackgroundType.Solid;
                
                Cell cell = worksheet.Cells["A1"];
                cell.PutValue("ThemeColor with Accent1 and 0.5 tint");
                cell.SetStyle(style);

                Console.WriteLine("ThemeColor constructor executed successfully with parameters (ThemeColorType.Accent1, 0.5)");
                Console.WriteLine($"ColorType: {themeColor.ColorType}, Tint: {themeColor.Tint}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ThemeColor constructor: {ex.Message}");
            }
            
            // Сохранить результат
            workbook.Save("ThemeColorCtorDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ThemeColorType](../../themecolortype/)
* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


