---
title: "StyleFlag.Borders"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Все настройки границ будут применены"
type: docs
url: /ru/net/aspose.cells/styleflag/borders/
---
## StyleFlag.Borders property

Все настройки границ будут применены.

```csharp
public bool Borders { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyBordersDemo
    {
        public static void Run()
        {
            // Создать книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создайте стиль с настройками границ
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].Color = System.Drawing.Color.Blue;

            // Создайте флаг стиля и включите границы
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;

            // Примените стиль к ячейке A1 только с границами
            cells["A1"].PutValue("Borders Demo");
            cells["A1"].SetStyle(style, styleFlag);

            // Сохраните книгу
            workbook.Save("BordersDemo.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


