---
title: "Font.SchemeType"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство Font. Получает и задает тип схемы шрифта"
type: docs
url: /ru/net/aspose.cells/font/schemetype/
---
## Font.SchemeType property

Получает и задает тип схемы шрифта.

```csharp
public FontSchemeType SchemeType { get; set; }
```

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertySchemeTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");

            Font font = cell.GetStyle().Font;
            font.SchemeType = FontSchemeType.Minor;
            font.Name = "Calibri";
            font.Size = 12;

            workbook.Save("FontSchemeTypeDemo.xlsx");
        }
    }
}
```

### См. также

* enum [FontSchemeType](../../fontschemetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


