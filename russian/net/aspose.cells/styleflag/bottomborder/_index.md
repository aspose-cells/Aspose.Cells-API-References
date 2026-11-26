---
title: "StyleFlag.BottomBorder"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Настройки нижней границы будут применены"
type: docs
url: /ru/net/aspose.cells/styleflag/bottomborder/
---
## StyleFlag.BottomBorder property

Настройки нижней границы будут применены.

```csharp
public bool BottomBorder { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyBottomBorderDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Создать стиль с настройками нижней границы
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.BottomBorder].Color = Color.Red;

            // Создайте флаг стиля и включите изменение нижней границы
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.BottomBorder = true;

            // Примените стиль с флагом к ячейке A1
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Cell with bottom border");
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


