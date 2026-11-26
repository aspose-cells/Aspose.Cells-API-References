---
title: "StyleFlag.RightBorder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Настройки правой границы будут применены"
type: docs
url: /ru/net/aspose.cells/styleflag/rightborder/
---
## StyleFlag.RightBorder property

Настройки правой границы будут применены.

```csharp
public bool RightBorder { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyRightBorderDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Создать стиль с границами
            Style borderStyle = workbook.CreateStyle();
            borderStyle.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            borderStyle.Borders[BorderType.RightBorder].Color = System.Drawing.Color.Red;

            // Создайте флаг стиля и включите правую границу
            StyleFlag borderFlag = new StyleFlag();
            borderFlag.RightBorder = true;

            // Применить стиль к ячейке
            Cell cell = worksheet.Cells["B2"];
            cell.SetStyle(borderStyle, borderFlag);

            // Сохраните книгу
            workbook.Save("RightBorderDemo.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


