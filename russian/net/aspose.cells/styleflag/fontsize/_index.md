---
title: "StyleFlag.FontSize"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Будет применена настройка размера шрифта"
type: docs
url: /ru/net/aspose.cells/styleflag/fontsize/
---
## StyleFlag.FontSize property

Настройка размера шрифта будет применена.

```csharp
public bool FontSize { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontSizeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Sample Text");

            Style style = workbook.CreateStyle();
            style.Font.Size = 18;
            style.Font.IsBold = true;

            StyleFlag styleFlag = new StyleFlag
            {
                FontSize = true,
                FontBold = true
            };

            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "A1");
            range.ApplyStyle(style, styleFlag);

            workbook.Save("FontSizeDemo.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


