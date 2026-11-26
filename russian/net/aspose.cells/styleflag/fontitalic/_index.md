---
title: "StyleFlag.FontItalic"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство StyleFlag. Настройка Font italic будет применена"
type: docs
url: /ru/net/aspose.cells/styleflag/fontitalic/
---
## StyleFlag.FontItalic property

Настройка курсивного шрифта будет применена.

```csharp
public bool FontItalic { get; set; }
```

### Примеры

```csharp
using System;
using System.Data;
using System.Drawing;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontItalicDemo
    {
        public static void Run()
        {
            // Создать новую книгу
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Создать примерные данные
            cells["A1"].PutValue("Product Name");
            cells["B1"].PutValue("Price");
            cells["A2"].PutValue("Laptop");
            cells["B2"].PutValue(1200);
            cells["A3"].PutValue("Monitor");
            cells["B3"].PutValue(250);

            // Создайте стили
            Style headerStyle = workbook.CreateStyle();
            headerStyle.Font.IsBold = true;
            headerStyle.Font.IsItalic = true;
            headerStyle.ForegroundColor = Color.LightGray;
            headerStyle.Pattern = BackgroundType.Solid;

            Style italicStyle = workbook.CreateStyle();
            italicStyle.Font.IsItalic = true;

            // Примените стили с StyleFlag
            Aspose.Cells.Range headerRange = cells.CreateRange(0, 0, 1, 2);
            StyleFlag headerFlag = new StyleFlag();
            headerFlag.FontBold = true;
            headerFlag.FontItalic = true;
            headerFlag.CellShading = true;
            headerRange.ApplyStyle(headerStyle, headerFlag);

            Aspose.Cells.Range dataRange = cells.CreateRange(1, 0, 2, 1);
            StyleFlag italicFlag = new StyleFlag();
            italicFlag.FontItalic = true;
            dataRange.ApplyStyle(italicStyle, italicFlag);

            // Сохраните книгу
            workbook.Save("FontItalicDemo.xlsx");
        }
    }
}
```

### См. также

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


