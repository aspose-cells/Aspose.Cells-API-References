---
title: "StyleFlag.TopBorder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Настройки верхней границы будут применены"
type: docs
url: /ru/net/aspose.cells/styleflag/topborder/
---
## StyleFlag.TopBorder property

Настройки верхней границы будут применены.

```csharp
public bool TopBorder { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyTopBorderDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создайте стиль с настройками верхней границы
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].Color = Color.Red;
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Dashed;

            // Создайте флаг стиля и включите изменение верхней границы
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.TopBorder = true;

            // Примените стиль к ячейке A1, включив только флаг верхней границы
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Sample Text");
            cell.SetStyle(style, styleFlag);

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


