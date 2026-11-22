---
title: "Font.SchemeType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Font. الحصول على أو تعيين نوع النظام للخط"
type: docs
url: /ar/net/aspose.cells/font/schemetype/
---
## Font.SchemeType property

يحصل على ويضبط نوع المخطط للخط.

```csharp
public FontSchemeType SchemeType { get; set; }
```

### أمثلة

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

### انظر أيضًا

* enum [FontSchemeType](../../fontschemetype/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


