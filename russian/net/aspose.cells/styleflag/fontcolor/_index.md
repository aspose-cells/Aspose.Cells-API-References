---
title: "StyleFlag.FontColor"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Настройка цвета шрифта будет применена"
type: docs
url: /ru/net/aspose.cells/styleflag/fontcolor/
---
## StyleFlag.FontColor property

Настройка цвета шрифта будет применена.

```csharp
public bool FontColor { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontColorDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            
            // Получить доступ к первому листу
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Создайте пользовательский стиль
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.BackgroundColor = System.Drawing.Color.LightGray;
            
            // Создайте флаг стиля и включите цвет шрифта и заливку ячейки
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontColor = true;
            styleFlag.CellShading = true;
            
            // Примените стиль к ячейке A1 с указанными флагами
            worksheet.Cells["A1"].PutValue("Red Text on Gray Background");
            worksheet.Cells["A1"].SetStyle(style, styleFlag);
            
            // Сохраните книгу
            workbook.Save("output.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


