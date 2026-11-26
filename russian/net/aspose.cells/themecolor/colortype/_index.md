---
title: "ThemeColor.ColorType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство ThemeColor. Получает и задает тип темы"
type: docs
url: /ru/net/aspose.cells/themecolor/colortype/
---
## ThemeColor.ColorType property

Получает и задает тип темы.

```csharp
public ThemeColorType ColorType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThemeColorPropertyColorTypeDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте два тематических цвета с разными типами
            ThemeColor color1 = new ThemeColor(ThemeColorType.Accent1, 0.5);
            ThemeColor color2 = new ThemeColor(ThemeColorType.Accent2, 0.3);
            
            // Продемонстрируйте свойство ColorType
            Console.WriteLine("Color1 Type: " + color1.ColorType);
            Console.WriteLine("Color2 Type: " + color2.ColorType);
            
            // Примените тематические цвета к ячейкам
            Style style1 = workbook.CreateStyle();
            style1.ForegroundThemeColor = color1;
            worksheet.Cells["A1"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundThemeColor = color2;
            worksheet.Cells["A2"].SetStyle(style2);
            
            // Сохраните книгу
            workbook.Save("ThemeColorDemo.xlsx");
        }
    }
}
```

### См. также

* enum [ThemeColorType](../../themecolortype/)
* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


